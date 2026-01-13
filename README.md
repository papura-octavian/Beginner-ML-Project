# Customer Churn Prediction (Beginner ML Project)

This is a **beginner-level machine learning project** created as a first hands-on step into applied ML.  
The goal is to understand the **full ML workflow**, not to build a production-grade system.

The project focuses on **customer churn prediction** using a classical, interpretable model.

---

## Problem Statement

Customer churn occurs when a customer stops using a service.  
From a business perspective, **missing a customer who is about to churn is more costly than raising a false alarm**.

This project answers the question:

> *Can we identify customers who are likely to churn, and understand why they leave?*

---

## Dataset

- **Dataset**: Telco Customer Churn  
- **Type**: Tabular data (numeric + categorical features)
- **Target variable**: `Churn` (Yes / No)

---

## Approach

The project follows a **clean, end-to-end ML pipeline**:

1. **Data preparation**
   - Type correction (`TotalCharges` converted to numeric)
   - Train / test split with stratification

2. **Preprocessing**
   - Missing value imputation (median / most frequent)
   - Feature scaling (StandardScaler)
   - One-hot encoding for categorical variables
   - Implemented via `ColumnTransformer` to avoid data leakage

3. **Model**
   - Logistic Regression (chosen for simplicity and interpretability)
   - Implemented inside a `Pipeline`

4. **Evaluation**
   - Precision, Recall, F1-score
   - Focus on **recall for churn (Yes)** due to business cost of false negatives

5. **Optimization**
   - Threshold tuning to prioritize recall
   - Final decision threshold: **0.3**

---

## Results

Using threshold tuning:

- **Churn Recall (Yes)**: ~**75%**
- The model successfully identifies **3 out of 4 customers who will churn**
- Accepts a controlled increase in false positives to reduce missed churn cases

---

## Business Insights

Key factors associated with higher churn:
- Month-to-month contracts
- Fiber optic internet service
- Higher total charges
- Lack of online security or tech support

Key factors associated with retention:
- Longer customer tenure
- Two-year contracts
- Lower monthly charges

---

## Technologies Used

- Python
- pandas
- NumPy
- scikit-learn
- Jupyter Notebook

---

## Project Status

🚧 **Learning project (early stage)**  
This is **not a final or production-ready system**.  
The purpose is to practice:
- ML pipelines
- Evaluation on imbalanced data
- Business-oriented metric selection (recall vs accuracy)

Further improvements (future work):
- Try tree-based models (Random Forest, XGBoost)
- Hyperparameter tuning
- Cross-validation
- Model persistence and deployment

---

## Author

Beginner ML project created as part of a personal learning journey.