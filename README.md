# Sepsis Prediction using Machine Learning

## Overview ##

This project focuses on predicting early-stage sepsis using machine learning techniques based on patient clinical data. It compares multiple machine learning models, selects the best-performing model, and provides explainable predictions using SHAP (SHapley Additive exPlanations).

## Features ##

Implementation of multiple machine learning models:

- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)

Automatic comparison and selection of the best-performing model

Feature scaling using StandardScaler

Model evaluation using:

- Accuracy
- ROC-AUC Score
- Confusion Matrix
- Classification Report

Interactive input system for entering patient clinical data

Risk assessment output (Low, Moderate, High)

Confidence level prediction

SHAP-based explanation of feature impact

Feature importance visualization

## Dataset ##

The project uses a synthetic dataset that simulates patient clinical parameters such as:

- Heart Rate (HR)
- Oxygen Saturation (O2Sat)
- Temperature
- Systolic Blood Pressure (SBP)
- Mean Arterial Pressure (MAP)
- Respiration Rate
- Creatinine
- Glucose
- Lactate
- Age

## Project Structure ##

Part_A_Training.ipynb – Trains multiple machine learning models, compares their performance, and saves the best model.

Part_B_Prediction.ipynb – Takes user input and predicts sepsis risk with SHAP-based explanation.

patient_data.csv – Synthetic dataset used for training.

README.md – Project documentation.

## How to Run ##

Run Part_A_Training.ipynb

- Loads and preprocesses the dataset
- Trains all machine learning models
- Evaluates model performance
- Selects the best-performing model
- Saves the trained model and required files (.pkl)

Run Part_B_Prediction.ipynb

- Loads the saved model
- Enter patient clinical details
- View prediction, probability, confidence level, and SHAP explanation

## Output ##

The system provides:

- Prediction (Sepsis / No Sepsis)
- Probability score
- Risk level classification
- Confidence level
- Clinical interpretation
- SHAP feature contribution graph
- Top contributing clinical features

## Notes ##

- Ensure that Part_A_Training.ipynb is executed before running Part_B_Prediction.ipynb.
- Keep all project files in the same directory.
- SHAP explanations may take slightly longer depending on the selected model.

## Future Improvements ##

- Integration with a web interface (Flask or Streamlit)
- Use of real-world medical datasets
- Hyperparameter tuning for improved performance
- Cloud deployment
- Integration with hospital management systems

## Author ##

Bhumi Sehrawat
