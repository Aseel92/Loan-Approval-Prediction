# Loan-Approval-Prediction
A machine learning project to predict loan approval status based on a customer's financial and personal details.

## Project Overview:
This project aims to build a predictive model that can assess a customer's eligibility for a loan. 

By analyzing a dataset containing various features such as income, credit history, and employment status, the model can predict whether a loan application is likely to be approved or rejected. 

This process can help financial institutions make faster and more informed decisions, reducing manual effort and potential bias.

## Dataset:
The dataset used in this project is loan_approval_dataset.csv, which contains a mix of categorical and numerical features.

The key features include:

Gender: Male/Female

Married: Yes/No

Dependents: Number of dependents

Education: Education_Graduate/Not Graduate

Self_Employed: Yes/No

ApplicantIncome: Applicant's income

CoapplicantIncome: Co-applicant's income

LoanAmount: The loan amount requested

Loan_Amount_Term: Term of the loan in months

Credit_History: Credit history meets guidelines (Yes/No)

Property_Area: Urban/Semiurban/Rural

The target variable is Loan_Status, which indicates whether the loan was approved ('Y') or rejected ('N').

## Workflow:

Data Loading and Exploration: The dataset is loaded, and initial exploratory data analysis is performed to understand feature distributions and relationships.

Data Preprocessing:
Feature Engineering: Categorical features are converted into a numerical format using Label Encoding.

Handling Imbalanced Data: 
The Loan_Status target variable is imbalanced. 
To address this, the Synthetic Minority Over-sampling Technique (SMOTE) is applied to create synthetic samples of the minority class, ensuring the model is not biased.

Model Selection and Training: Several classification models are trained on the preprocessed data:
Logistic Regression and Decision Tree Classifier

Model Evaluation: Each model's performance is evaluated using metrics such as Accuracy, Precision, Recall, and F1-Score. 
A Confusion Matrix is also generated for each model to visualize its performance in detail.

Results
The Decision Tree Classifier model achieved the highest accuracy, demonstrating its effectiveness in predicting loan approval status. 
The use of SMOTE helped ensure robust performance on the imbalanced dataset.
