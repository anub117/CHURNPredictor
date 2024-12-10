Churn Predictor
This project predicts customer churn using machine learning. The workflow includes data preprocessing, exploratory data analysis (EDA), handling class imbalance, training multiple models, and making predictions with a saved model.

Overview
The project uses the Telco Customer Churn dataset to predict whether a customer will churn based on various features. The key steps include:

Data Preprocessing: Cleaning, handling missing values, and encoding categorical variables.
EDA: Generating visualizations like histograms, box plots, and heatmaps.
Class Imbalance Handling: Using SMOTE to balance the dataset.
Model Training: Training Decision Tree, Random Forest, and XGBoost models.
Inference: Saving and loading models for predicting churn for new customer data.
Files in this Repository
WA_Fn-UseC_-Telco-Customer-Churn.csv: Dataset used for training and testing.
churn_predictor.ipynb: Jupyter notebook with the complete code for preprocessing, visualization, training, and evaluation.
encoders.pkl: Pickled label encoders for categorical features.
customer_churn_model.pkl: Pickled trained Random Forest model and feature information.
README.md: Project description and instructions.
requirements.txt: List of Python dependencies.
