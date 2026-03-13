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
The models were evaluated based on their ability to classify the three credit tiers. Below are the comparative results:

| Model | Accuracy | Precision | Recall | F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| **XGBoostClassifier** | 0.82 | 0.82 | 0.82 | 0.82 |
| **RandomForestClassifier** | 0.80 | 0.80 | 0.80 | 0.80 |
| **GradientBoostingClassifier** | 0.76 | 0.77 | 0.76 | 0.76 |
| **AdaBoostClassifier** | 0.71 | 0.71 | 0.71 | 0.71 |

## XGBoost emerged as the best performing model for this dataset.
