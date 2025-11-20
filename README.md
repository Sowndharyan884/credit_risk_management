# Credit Risk Prediction with Explainable AI (XGBoost, SHAP, LIME)

This project builds a credit risk prediction model using a tuned XGBoost classifier with full explainability through SHAP and LIME. The objective is to classify borrowers as defaulters or non-defaulters, while ensuring transparency, fairness, and reliability for financial decision-making.

---

## Project Overview

Financial institutions require models that are both accurate and interpretable. This project delivers a high-performance machine learning model along with global and local explanations that justify predictions.

Key components:
- XGBoost classifier with hyperparameter tuning
- Complete preprocessing pipeline
- Global explainability using SHAP
- Local, instance-level explanation using LIME
- Business insights for risk teams

---

## Model Performance (Test Set)

- Test AUC: 0.9504
- Test Accuracy: 0.9334
- Precision (default class): 0.9507
- Recall (default class): 0.7328
- F1-score (default class): 0.8276

The model exceeds industry standards and meets all academic requirements.

---

## Features of the Project

### 1. Data Preprocessing
- Handling missing values
- Scaling numeric columns
- Encoding categorical variables
- Implemented using ColumnTransformer and Pipeline

### 2. Model Development
- XGBoost Classifier
- Hyperparameter tuning using RandomizedSearchCV
- Evaluation through:
  - AUC
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Confusion matrix
  - Classification report

### 3. Global Explainability (SHAP)
- SHAP summary plot
- Top 10 important features
- SHAP dependence plots (top 3 features)

### 4. Local Explainability (LIME)
Explanations generated for 5 borrowers:
- 2 defaulters
- 2 non-defaulters
- 1 borderline case

---

## Project Structure

Credit_Risk_Analysis/
│
├── Credit_card_final_submission.ipynb
├── credit_risk_dataset.csv
└── README.md

---

## Key Insights for CRO (Chief Risk Officer)

- Affordability indicators such as interest rate, loan amount, and loan_percent_income strongly influence default risk.
- Stability indicators like borrower income, employment length, and credit history reduce default probability.
- SHAP provides global feature importance, while LIME supports case-level explanations.
- Model is suitable for credit approval, risk-based pricing, and portfolio monitoring.

---

## How to Run the Project

### 1. Clone the repository
git clone https://github.com/your-username/credit-risk-analysis.git
cd credit-risk-analysis

### 2. Install dependencies
pip install -r requirements.txt

### 3. Run the notebook
jupyter notebook Credit_card_final_submission.ipynb

---

## Requirements (requirements.txt)

xgboost  
shap  
lime  
pandas  
numpy  
matplotlib  
seaborn  
scikit-learn  

---

## Contact
Sowndharyan  
Aspiring AI Engineer & Python Developer

