# Data-Science-Project
# Diabetes Prediction API 

Developed using the Pima Indians Diabetes dataset from Kaggle, this project builds a complete pipeline—from data preprocessing and machine learning model training to API deployment using **FastAPI**.

---

## 📦 Repository Structure
pima-diabetes-api/
├── data/
│ └── diabetes.csv # Raw dataset from Kaggle
│
├── notebooks/
│ └── diabetes_modeling.ipynb # EDA, preprocessing, model training
│
├── app/
│ └── diabetes_model.pkl # Trained model + scaler using joblib
|
└── README.md # This documentation


---

## 🎯 Project Overview

- **Objective**: Predict whether a patient has diabetes based on diagnostic variables.
- **Dataset**: 768 female patients (age ≥ 21, Pima Indian heritage) with features like `Pregnancies`, `Glucose`, `BloodPressure`, `BMI`, etc.:contentReference[oaicite:1]{index=1}
- **Pipeline**:
  1. Load and preprocess data (handle zeros, impute/missing).
  2. Train machine learning models (e.g., Logistic Regression, Random Forest).
  3. Evaluate using accuracy, precision, recall, F1-score.
  4. Save the best model and scaler.
  5. Deploy API for inference with FastAPI.

---

# 🧪 API Usage
Endpoint: predict_diabetes
Method: POST

# *Payload (example):*
{
  "Pregnancies": 3,
  "Glucose": 120,
  "BloodPressure": 70,
  "SkinThickness": 20,
  "Insulin": 79,
  "BMI": 25.0,
  "DiabetesPedigreeFunction": 0.5,
  "Age": 33
}
# *Response:*
{
  "prediction": 1,  // 1 = diabetic, 0 = non-diabetic
  "probability": 0.84
}


# Dataset : https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database

# Diabetes predictor:
<img width="1432" height="1351" alt="Image" src="https://github.com/user-attachments/assets/2ca2eea0-c168-4d0b-9769-f52be3a8c74a" />


# Diabeties Result:

<img width="404" height="80" alt="Image" src="https://github.com/user-attachments/assets/f4a38d23-d3f5-4b09-923c-556b18758aa8" />


Project by Nisha under CODTECH Internship
