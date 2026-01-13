# Beginner Machine Learning Projects (Tabular Data)

This repository contains a collection of **beginner-level machine learning projects** built to practice the full ML workflow on **different tabular datasets**.

Each notebook focuses on a new dataset but follows the same core structure:
- clean preprocessing
- leakage-safe pipelines
- simple, interpretable models
- correct evaluation metrics

The goal is **learning and consistency**, not production-grade systems.

---

## Included Projects

### 1) Customer Churn Prediction
**Task:** Binary classification  
**Goal:** Predict whether a customer will churn

**Highlights:**
- ColumnTransformer + Pipeline (leakage-safe)
- Logistic Regression
- Threshold tuning to improve recall on churned customers
- Business-oriented interpretation

---

### 2) Student Performance Prediction
**Task:** Classification / Regression (depending on target)  
**Goal:** Predict student academic performance based on demographic and study-related features

**Highlights:**
- Handling categorical + numeric features
- Feature scaling and encoding
- Interpretable baseline model
- Focus on understanding feature impact on performance

---

## Common ML Workflow Used
All notebooks follow the same end-to-end structure:

1. Dataset exploration & cleaning  
2. Train / test split  
3. Preprocessing with `ColumnTransformer`  
4. Model training (baseline first)  
5. Evaluation (precision, recall, F1, or regression metrics)  
6. Interpretation of results  

This makes the repository easy to **extend with new datasets**.

---

## Repository Structure
```

Beginner-ML-Project/
│
├── churn.ipynb                # Customer churn project
├── StudentPerformance.ipynb   # Student performance project
└── README.md

```

---

## Tech Stack
- Python
- pandas, NumPy
- scikit-learn
- Jupyter Notebook

---

## How to Run
1. Clone the repository
2. Install dependencies:
   - `pip install pandas numpy scikit-learn jupyter`
3. Run:
   - `jupyter notebook`
4. Open any notebook and run cells top-to-bottom

---

## Project Status
Ongoing learning repository.  
New notebooks will be added for different datasets and ML tasks (classification & regression).

## Author
Created as part of a personal machine learning learning journey.