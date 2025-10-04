# Airline Customer Satisfaction Prediction

## Project Overview
This project predicts airline passenger satisfaction using demographic information, flight details, and onboard service ratings. The goal is to help airlines understand key factors affecting satisfaction and improve the overall customer experience.

## Dataset
- **Source:** [Kaggle - Airline Customer Satisfaction](https://www.kaggle.com/datasets/raminhuseyn/airline-customer-satisfaction)  
- **Rows:** 129,880  
- **Columns:** 22  
- **Target Variable:** `satisfaction` (binary: 'neutral or dissatisfied' vs. 'satisfied')

## Data Preprocessing
- Converted categorical features (`Customer Type`, `Type of Travel`, `Class`) to numeric/ordinal encodings.  
- Encoded target variable `satisfaction` as 0 (neutral/dissatisfied) and 1 (satisfied).  
- Handled missing values: median for numeric columns, mode for categorical.  
- Scaled numerical features where appropriate.  

## Feature Engineering
- Derived additional features if needed, such as total delays or average service rating.  

## Modeling
- Models implemented:  
  - Logistic Regression  
  - Random Forest Classifier  
  - Support Vector Classifier (SVC)  
  - Gradient Boosting 
  ....etc
- Hyperparameter tuning performed using `RandomizedSearchCV`.  
- Evaluation metrics: Accuracy, F1-Score  
