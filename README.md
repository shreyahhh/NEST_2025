# 🧠 Predicting Recruitment Rate in Clinical Trials using Machine Learning

![NEST2025 - NOVARTIS](https://github.com/user-attachments/assets/3c96b0c4-463b-4f94-a451-5bca5b741ab4)


> **Team NO DIRECTION | Bennett University**  
> Project under NEST: Nurturing Excellence, Strengthening Talent  
> **Date**: January 26, 2025

---

## 📘 Overview

Recruitment rates are crucial for the success of clinical trials, impacting cost, duration, and trial outcomes. Traditional methods often ignore real-world variables like competition or geographic diversity. In this project, we propose a **data-driven machine learning framework** to predict **Recruitment Rate (RR)** using structured and unstructured data.

---

## 🛠️ Methodology

### 🔹 Data Preprocessing
- Removed irrelevant columns and handled missing values
- Standardized location names using `fuzzywuzzy` and `rapidfuzz`
- Derived features such as number of cities, countries, and sites

### 🔹 Feature Engineering
- One-hot encoding and label encoding for categorical features
- BERT-based embeddings for textual data (Conditions, Interventions, Locations)
- Log-transform to reduce skewness in numeric features

### 🔹 Model Development
- Models used: Random Forest, Gradient Boosting, XGBoost, Linear Regression
- Tuned using GridSearchCV (e.g., `max_depth=20`, `n_estimators=950`)
- Evaluated via R² and MSE with 5-fold cross-validation

---

## 📊 Results

### 🎯 Key Metrics
- **R²** = 0.63
- **MSE** = 0.46
- Neural networks outperformed baselines due to embedding capabilities

### 📌 Key Predictors
1. Enrollment target
2. Age groups
3. Trial duration
4. Trial phase
5. Study design factors

### 📈 Feature Importance

![Feature Importance](https://raw.githubusercontent.com/your-username/your-repo/main/assets/feature_importance.png)

---

### 🔍 Actual vs Predicted
![Actual vs Predicted](https://github.com/user-attachments/assets/0e535851-056c-40e7-b388-cffb8c274d92)

---

## 🔮 Future Work

- Incorporate **LLMs** to dynamically predict RR from live trial data
- Enhance embeddings for sparse/rare data cases
- Include granular demographic details
- Improve explainability using **SHAP values**

---

## 🧑‍💻 Team Members
- Swayam Prasad Sah  
- Shreya  
- Ananya Verma  
- Aman Gupta  
- Pritesh Punj

---

