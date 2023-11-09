# XGBoost on Telco Customer Churn

## Overview
This GitHub repository features a Python implementation of an XGBoost model designed for predicting customer churn in a telecommunications dataset. The model utilizes various features, including Monthly Charges, Total Charges, and Tenure Months.

## Dataset

The dataset used in this project is "Telco_customer_churn.csv" and it was collected from the kaggle website: https://www.kaggle.com/datasets/yeanzc/telco-customer-churn-ibm-dataset

## Data Exploration & Cleaning
- Explored dataset details, dimensions, and descriptive statistics.
- Removed unnecessary columns like 'Churn Label', 'Churn Score', 'CLTV', 'Churn Reason'.
- Eliminated columns with only one unique value.
- Replaced blank spaces in the 'City' column and column names with underscores.
- Checked for missing and duplicated data.
- Replaced blank spaces in 'Total Charges' with 0.
- Converted 'Total Charges' to numeric after addressing blank spaces.
- Applied one-hot encoding to categorical columns.

## XGBoost Modeling
- Checked dataset balance, noting around 27% customer churn.
- Split data into training and test sets with stratification.
- Utilized XGBoost and Random Forest classifiers.
- Conducted hyperparameter tuning using GridSearchCV.
- Evaluated models using cross-validation and calculated F1 scores.

## Results
- Achieved an F1 score of X% on the final XGBoost model.
- Revealed a confusion matrix indicating more false negatives (Type II errors) than false positives (Type I errors).
- Identified the most important features using XGBoost's feature importance plot.

## Usage
1. Clone the repository.
2. Install the required libraries.
3. Run the Jupyter notebook for a step-by-step walkthrough of the code.

