# Design of Customer Churn Prediction Project

## 1. Dataset
- Telco Customer Churn dataset
- Columns: customerID, gender, tenure, MonthlyCharges, Churn, etc.

## 2. Data Cleaning
- Convert TotalCharges to numeric
- Fill missing values
- Encode target variable (Churn)
- Convert categorical features to numeric via one-hot encoding

## 3. Model
- Logistic Regression (baseline)
- Balanced Logistic Regression for high churn recall
- Final model: Pipeline with StandardScaler + Logistic Regression (class_weight='balanced')

## 4. Evaluation
- Metrics: Accuracy, Precision, Recall, F1-score
- Confusion Matrix for visual interpretation

## 5. Insights
- Top features affecting churn: tenure, MonthlyCharges, Contract type
- Business reasoning: Early detection of churn reduces revenue loss