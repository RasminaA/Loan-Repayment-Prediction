# Loan Repayment Prediction

## Overview

This project uses machine learning classification techniques to predict loan repayment status based on applicant and loan-related features.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Google Colab

## Project Workflow

1. Data loading and exploration
2. Missing-value analysis and handling
3. Duplicate checking
4. Exploratory data analysis
5. Categorical variable encoding
6. Feature engineering
7. Train-test split
8. Classification model training
9. Model evaluation
10. Hyperparameter tuning

## Feature Engineering

Two additional features were created:

- **TotalIncome** – Combined applicant and co-applicant income
- **Income_Loan_Ratio** – Total income relative to the loan amount

## Models Used

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Gradient Boosting Classifier
- XGBoost Classifier

## Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- ROC-AUC
- Log Loss
- F1-score

## XGBoost Results

On the test set of 123 samples, XGBoost achieved:

- **Accuracy:** 0.74
- **Precision:** 0.76
- **Recall:** 0.88
- **F1-score:** 0.81 for class 1

## Hyperparameter Tuning

Random Forest hyperparameters were optimized using GridSearchCV with 5-fold cross-validation.

Best parameters:

- `n_estimators`: 200
- `max_depth`: 10
- `min_samples_split`: 2

Best cross-validation ROC-AUC score:

**0.8018**

## Dataset

The dataset contains applicant information, income details, loan information, credit history, property area, and loan status.

## Project Output

The trained classification models generate loan repayment predictions and probability estimates for the test data.
