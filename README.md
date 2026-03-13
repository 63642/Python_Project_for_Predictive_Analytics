# Credit_Score_Prediction_Machine_Learning_Project

## Project Overview
#### This project aims to automate the process of classifying customer credit scores into categories (e.g., Good, Standard, Poor). By leveraging historical financial data and banking behavior, we built a robust machine learning pipeline that handles complex data cleaning, feature engineering, and high-performance classification.


## Dataset Description
#### The model is trained on a comprehensive financial dataset consisting of 100,000 records for training and 50,000 records for testing.
#### Target Variable: Credit_Score

#### Key Features:
- Financials: Annual Income, Monthly In-hand Salary, Outstanding Debt.
- Banking Habits: Number of Bank Accounts, Number of Credit Cards, Interest Rate, Delay from due date.
- Credit History: Credit History Age, Number of Credit Inquiries, Credit Mix.
- Behavioral: Monthly Balance, Payment Behaviour, Amount Invested Monthly.

## Data Preprocessing & Engineering
#### A significant portion of this project focuses on data quality and feature transformation:
- Anomaly Detection: Cleaned structural errors in categorical fields like Occupation, SSN, and Payment_Behaviour using customer-specific mode imputation.
- Numerical Cleaning: Handled "dirty" numerical strings (e.g., stripping non-numeric characters from Age and Annual_Income).
- Feature Transformation: Converted Credit_History_Age from strings (e.g., "22 years and 1 month") into a continuous float format (22.01) for model compatibility.
- Imputation Strategy: Used median and mode values grouped by Customer_ID to preserve individual financial profiles.

## Model Architecture
#### The project explores several ensemble learning techniques to find the most accurate classifier:
- Random Forest Classifier
- Gradient Boosting (GBM)
- AdaBoost
- XGBoost (Optimized for high performance)

## Results & Evaluation
#### The models were evaluated using standard classification metrics:
- Accuracy: Overall correctness of the prediction.
- F1-Score: To ensure a balance between precision and recall across all credit classes.
- Classification Report: Detailed breakdown of performance per class.


## Model Performance Evaluation
After extensive data cleaning and feature engineering, four major classification models were tested. **XGBoost** emerged as the most balanced and accurate model for this dataset.

| Model | Accuracy | Precision | Recall | F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| **XGBoostClassifier** | **0.7470** | **0.7477** | **0.7470** | **0.7470** |
| RandomForestClassifier | 0.7386 | 0.7658 | 0.7386 | 0.7426 |
| GradientBoostingClassifier | 0.7239 | 0.7255 | 0.7239 | 0.7236 |
| AdaBoostClassifier | 0.6460 | 0.6474 | 0.6484 | 0.6450 |
