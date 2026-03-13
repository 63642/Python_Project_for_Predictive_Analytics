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
Anomaly Detection: Cleaned structural errors in categorical fields like Occupation, SSN, and Payment_Behaviour using customer-specific mode imputation.
Numerical Cleaning: Handled "dirty" numerical strings (e.g., stripping non-numeric characters from Age and Annual_Income).
Feature Transformation: Converted Credit_History_Age from strings (e.g., "22 years and 1 month") into a continuous float format (22.01) for model compatibility.
Imputation Strategy: Used median and mode values grouped by Customer_ID to preserve individual financial profiles.
