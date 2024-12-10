# Customer Churn Prediction Using Machine Learning

## Overview
This project aims to predict customer churn in the telecom industry using machine learning models. By analyzing customer demographics, account information, and usage patterns, we can identify customers likely to leave and take proactive measures to retain them.

---

## Dataset
- **Source**: WA_Fn-UseC_-Telco-Customer-Churn.csv
- **Description**: 
  - The dataset contains 7,043 customer records with 21 columns including demographic details, service subscriptions, account information, and churn status.
- **Target Variable**: 
  - `Churn`: Indicates whether the customer has churned (`Yes`/`No`).

---

## Features
1. **Numerical**:
   - `tenure`, `MonthlyCharges`, `TotalCharges`
2. **Categorical**:
   - `gender`, `SeniorCitizen`, `Partner`, `Dependents`, `PhoneService`, etc.

---

## Tools and Libraries
- Python Libraries:
  - `numpy`, `pandas`, `matplotlib`, `seaborn`
  - `scikit-learn`, `imblearn`, `xgboost`, `pickle`

---

## Workflow

### 1. Data Preprocessing
- Dropped `customerID` column as it is not relevant for modeling.
- Handled missing values in `TotalCharges` by replacing spaces with `0.0` and converting to a numeric data type.
- Applied label encoding to categorical features for compatibility with machine learning models.

### 2. Exploratory Data Analysis (EDA)
- Visualized the distribution of numerical features using histograms and box plots.
- Analyzed correlations between numerical features using a heatmap.
- Visualized the class distribution of categorical features and the target variable.

### 3. Handling Imbalanced Data
- Used SMOTE (Synthetic Minority Oversampling Technique) to balance the target class distribution in the training data.

### 4. Model Training and Evaluation
- Implemented three machine learning models:
  - Decision Tree
  - Random Forest
  - XGBoost
- Performed 5-fold cross-validation to evaluate model performance.
- Evaluated the best model (Random Forest) on the test set using:
  - Accuracy Score
  - Confusion Matrix
  - Classification Report

### 5. Saving the Model
- Saved the trained Random Forest model and feature encoders as pickle files for future use.

### 6. Predicting Churn
- Preprocessed input data using the saved encoders.
- Used the trained model to predict churn status and probability.
---
