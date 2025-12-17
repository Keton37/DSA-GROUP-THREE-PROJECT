# DSA-GROUP-THREE-PROJECT

- Kariuki Irene -675467
- Nafisa Amirali - 674653
- Tita Claudlynne -674071
- Petro Aimata - 675208


This project predicted customer churn to help businesses identify customers who are likely to leave and take action to retain them.
# Customer Churn Prediction
We use a dataset from Kaggle and follow a structured week-by-week workflow, covering data exploration, cleaning, feature engineering, model training, and evaluation.

## Dataset Information

Source: Kaggle – Customer Churn Dataset

Rows: 7,043 customers

Columns: 21 features

Target Variable: Churn

Yes → Customer left

No → Customer stayed

## Key Features

Customer demographics (Gender, SeniorCitizen, Partner, Dependents)

Services (InternetService, OnlineSecurity, TechSupport, StreamingTV, etc.)

Contract & payment details (Contract, PaymentMethod, MonthlyCharges, TotalCharges)

## Tools & Technologies

Programming Language: Python

Libraries Used:

Pandas, NumPy

Matplotlib, Seaborn

Scikit-learn

Joblib

## Project Workflow

###🔹 Week 1: Project Introduction & Data Setup

Loaded dataset using Pandas

Previewed data (head())

Inspected structure (info())

Generated summary statistics (describe())

###🔹 Week 2: Data Exploration & Cleaning

Exploratory Data Analysis (EDA):

Churn distribution

Tenure vs Churn

Monthly charges distribution

Contract type vs Churn

Payment method vs Churn

Internet service vs Churn

Data Cleaning:

Dropped customerID

Converted Churn to numeric (Yes = 1, No = 0)

Filled missing values:

Numerical → Median

Categorical → Mode

Encoded categorical variables using Label Encoding

Standardized numerical features using StandardScaler

###🔹 Week 3: Feature Engineering & Data Splitting

Final feature set created

Target variable separated

Train-test split:

80% Training

20% Testing

Stratified on Churn to handle class imbalance

###🔹 Week 4: Model Building

Two machine learning models were trained:

1️⃣ Logistic Regression

Solver: saga

max_iter = 5000

Suitable for binary classification

2️⃣ Random Forest Classifier

Ensemble-based model

Handles non-linear relationships well

Provides feature importance

###🔹 Week 5: Model Evaluation & Reporting
📈 Evaluation Metrics

Accuracy

Precision

Recall

F1-Score

Confusion Matrix

Classification Report

### 🔍 Results Summary
Model	Accuracy	Precision	Recall	F1-Score
Logistic Regression	73.9%	68.8%	2.9%	0.06
Random Forest	78.9%	63.0%	49.2%	0.55

✅ Random Forest performed better, especially in detecting churned customers (higher recall and F1-score).

### 📊 Feature Importance

Random Forest feature importance analysis shows that variables such as:

Contract

tenure

MonthlyCharges

TotalCharges

InternetService

play a significant role in predicting churn.


