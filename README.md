# 🌱 Agricultural Intelligence (AI)

*By Team Crop-timists*

## 📖 Overview

This project implements three machine learning modules to support data-driven farming decisions through a unified web interface built with Flask.

1. Crop Recommendation – Suggests the most suitable crop based on soil nutrients (N, P, K), weather conditions (temperature, humidity, pH, rainfall).
2. Crop Yield Prediction – Predicts yield (MT/ha) based on crop, state, year, rainfall, fertilizer, pesticide use, and cultivated area.
3. Crop Profitability Analysis – Estimates profitability percentage and indicates whether a crop is profitable or not profitable.

The web application integrates all three modules into an intuitive UI.

---

## 📂 Directory Structure

agriculture-ai    
│── app.py                        # Main Flask app        
│  
├── models/                       # ML models & data files (⚠️ crop_yield_prediction_model.pkl excluded due to large size)   
│   │── Crop_recommendation.csv    
│   │── crop_yield.csv     
│   │── crop_value_cost_data.xlsx    
│   │── crop_recommendation_model.pkl    
│   │── crop_profitability_model.pkl     
│   │── Python files of all the three models (for training the models)    
│   └── label_encoders pickle files    
│     
├── static/                       # Static assets      
│   └── background.jpg     
│      
└── templates/ index.html                 # Frontend HTML       
    

---

## ⚙️ Setup Instructions   

### 1. Download the zipped folder. Extract all the files.

### 2. Install Dependencies

Flask==3.0.3    
Jinja2==3.1.4     
Werkzeug==3.0.3     
pandas==2.2.2    
numpy==1.26.4     
scikit-learn==1.5.1    
openpyxl==3.1.5     

### 3. Create a project folder. Start by running the crop_yield_prediction_model.py file to save its .pkl file.

### 4. Run Flask App

python app.py

### 5. Open in Browser

👉 http://127.0.0.1:5000/

---

## 🖼️ Screenshots

### 🌱 Crop Recommendation

<img width="1891" height="875" alt="image" src="https://github.com/user-attachments/assets/f93d3a16-2b0d-452d-a518-bfcbcf9ea237" />

### 🌾 Crop Yield Prediction

<img width="1879" height="925" alt="image" src="https://github.com/user-attachments/assets/725bbd54-79c7-4928-a633-0cacd1936309" />

### 💰 Crop Profitability Analysis

<img width="1883" height="871" alt="image" src="https://github.com/user-attachments/assets/3ca6288a-8e7d-40e2-b850-93099ef98460" />

### 📊 Input Value Ranges

<img width="1892" height="381" alt="image" src="https://github.com/user-attachments/assets/26ee5c39-80bf-4c38-bf72-7ef4cb4e4c2b" />

---

## 🧪 Training & Testing the Models

Use 'Agricultural Inteligence (AI).ipynb' file uploaded separately for cleaning the raw data, visualization, training & testing the models and checking its accurracy.

---

## 🎯 Features

* Integrated web dashboard for three ML models
* Dropdowns for selecting crops, states, and years (1997–2026)
* Auto-prefilled rainfall/area between yield → profitability
* Clear result formatting (green = profitable & red = not profitable)
* Background image and styled cards for UI polish
