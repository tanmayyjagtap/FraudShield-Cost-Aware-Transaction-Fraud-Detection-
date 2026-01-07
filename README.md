# FraudShield – Transaction Fraud Detection

FraudShield is a machine learning-based fraud detection system designed to identify fraudulent financial transactions with high accuracy and minimal business loss.

## Project Overview
The project uses transaction-level data to detect fraud in mobile financial transactions. It includes exploratory data analysis, feature engineering, model comparison, threshold optimization, and a demo user interface.

## Dataset
- Transactions: 11,142
- Target variable: isFraud (0 = Legitimate, 1 = Fraud)
- Fraud rate: ~10.25%

## Methodology
- Exploratory Data Analysis (EDA)
- Feature engineering (time-based and balance-based features)
- Model comparison:
  - Logistic Regression
  - Random Forest
  - XGBoost
- Performance evaluation using Precision, Recall, F1-score, and ROC-AUC
- Cost-based threshold optimization to minimize financial loss

## Final Model Performance
- Model: XGBoost
- ROC-AUC: 0.99999
- Accuracy: 99.96%
- Precision (Fraud): 1.00
- Recall (Fraud): 0.9956

At an optimized threshold of 0.01:
- False Negatives: 0
- False Positives: 11
- Estimated loss reduced by ~1.03 million (relative to default threshold)

## Demo
An interactive UI (Gradio) allows users to enter transaction details and receive
