# Financial Fraud Detection Project

A machine learning project to detect fraudulent users on an online gambling platform using real behavioural data.

---

## Overview
- Combines **customer**, **payment**, and **login** datasets  
- Cleans data and engineers behaviour-based features  
- Trains an **XGBoost** model for binary fraud classification  
- Uses **SHAP** to interpret model predictions  

---

## Key Behaviour Features
- Shared registration IP and registration channel  
- Days from registration to first transaction  
- PAYIN count and amount within 7 days  
- Night-time and high-frequency PAYINs  
- Login activity in the first 7 days  
- Log-transformed indicators for skewed variables  

---

## Model
- Algorithm: **XGBoostClassifier**  
- Evaluation: **AUC ≈ 0.986** (5-fold CV), strong recall on fraud class  
