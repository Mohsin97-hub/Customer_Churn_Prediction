# 📉 Customer Churn Prediction

This project focuses on predicting customer churn using various machine learning models such as Logistic Regression, Random Forest, Gradient Boosting, and Support Vector Machines (SVM). It is part of a hands-on data science internship task focused on real-world telecom data.

---

## 🔍 Problem Statement
Telecom companies lose significant revenue due to customer churn. The goal is to develop a predictive model that can identify customers likely to churn so the company can take proactive retention measures.

---

## 📁 Dataset
The dataset contains customer-level information such as:
- Demographics (e.g., gender, age)
- Services used (e.g., phone, internet, streaming)
- Account details (e.g., tenure, billing type)
- Churn (target variable)

---

## 🧪 Steps Covered

### 1. Data Exploration and Cleaning
- Handled missing values
- Performed EDA (distributions, outliers, correlations)
- Converted categorical variables using encoding
- Converted `True/False` to `1/0`

### 2. Feature Engineering
- Created derived features like `Tenure in Years`
- Selected meaningful features for modeling

### 3. Model Training & Tuning
- Trained multiple models:
  - Logistic Regression
  - Random Forest
  - Gradient Boosting
  - Support Vector Machine
- Applied **SMOTE** to balance class distribution
- Hyperparameter tuning using **GridSearchCV**

### 4. Evaluation Metrics
- Accuracy, Precision, Recall, F1 Score
- ROC-AUC Score
- Confusion Matrix
- Classification Report

---

## 🧠 Best Performing Model
🎯 **Tuned Random Forest**
- ROC AUC: `0.81` (train) → `0.56` (test)
- Accuracy: 63%
- Best hyperparameters: `n_estimators=100`, `max_depth=10`, `min_samples_split=2`, `min_samples_leaf=1`

---

## 📈 Final Results Snapshot (Test Set)
| Metric       | Value   |
|--------------|---------|
| Accuracy     | 63.13%  |
| Precision    | 38.15%  |
| Recall       | 22.65%  |
| F1 Score     | 28.43%  |
| ROC-AUC      | 0.5688  |

---

## 📌 Key Insights
- The data was highly imbalanced — handled using SMOTE.
- The `Tenure`, `MonthlyCharges`, and `Contract` type were strong churn indicators.
- Logistic Regression gave stable baseline results.
- Random Forest performed best after tuning, although the test performance dropped (indicating some overfitting).

---

## 📂 Files in This Repo
- `Customer_Churn_Prediction.ipynb`: The main Jupyter notebook
- `final_model.pkl`: Trained model file
- `churn_data.csv`: Dataset
- `Churn_Presentation.pdf`: Business presentation with findings

---

## 🚀 Tools Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- SMOTE (from imbalanced-learn)

---

## 📊 Business Recommendation
Focus retention efforts on customers with month-to-month contracts, high monthly charges, and shorter tenure. These are the most likely to churn.

---

## 🧑‍💻 Author
**Mohsin Khan** — Aspiring Data Scientist | Data Analytics Intern  
[www.linkedin.com/in/mohsin-khan-12b797342](#) • [Mohsin97-hub](#) • [mohsinkhanmk0085@gmail.com](#)

