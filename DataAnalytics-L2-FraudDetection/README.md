# 💳 Fraud Detection Using Machine Learning

> **Oasis Infobyte (OIBSIP) • Data Analytics Internship • Level 2 – Task 3**

An end-to-end Machine Learning project that detects fraudulent credit card transactions using **Logistic Regression**, **Random Forest**, and **SMOTE** to handle severe class imbalance.

---

## 📌 Project Overview

Financial fraud causes billions of dollars in losses every year. Since fraudulent transactions are extremely rare, traditional accuracy-based models often fail to identify them.

This project builds a complete fraud detection pipeline that:

- Cleans and analyzes real transaction data
- Handles imbalanced classes using **SMOTE**
- Trains two machine learning models
- Evaluates performance using fraud-specific metrics
- Recommends the best model for deployment

---

## 🎯 Objective

Develop a reliable fraud detection system capable of identifying fraudulent credit card transactions while minimizing missed fraud cases through proper machine learning techniques.

---

## 🛠 Tech Stack

| Category | Tools |
|----------|------|
| Language | Python |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Imbalanced Learning | SMOTE (imblearn) |
| Development | Google Colab |

---

## 📂 Dataset

**Dataset:** Credit Card Fraud Detection Dataset

**Source:** Kaggle (European Cardholders)

| Feature | Value |
|---------|------:|
| Transactions | 284,807 |
| Features | 31 |
| Fraud Cases | 492 |
| Target Column | `Class` |

**Target Labels**

- **0** → Genuine Transaction
- **1** → Fraudulent Transaction

---

## 🚀 Project Workflow

```text
Dataset
   │
   ▼
Data Cleaning
   │
   ▼
Exploratory Data Analysis
   │
   ▼
Class Imbalance Analysis
   │
   ▼
SMOTE Oversampling
   │
   ▼
Train/Test Split
   │
   ▼
Machine Learning Models
   │
   ├── Logistic Regression
   └── Random Forest
   │
   ▼
Performance Evaluation
   │
   ▼
Business Insights
```

---

## ✨ Features Implemented

- ✅ Data inspection & preprocessing
- ✅ Duplicate and missing value handling
- ✅ Fraud vs Genuine transaction analysis
- ✅ Transaction amount distribution
- ✅ Time-of-day transaction analysis
- ✅ Class imbalance visualization
- ✅ SMOTE oversampling
- ✅ Logistic Regression classifier
- ✅ Random Forest classifier
- ✅ Confusion Matrix
- ✅ ROC-AUC comparison
- ✅ Feature Importance analysis
- ✅ Business recommendations

---

## 🤖 Machine Learning Models

| Model | Purpose |
|--------|----------|
| Logistic Regression | Baseline fraud classification |
| Random Forest | Ensemble model for improved fraud detection |

---

## 📊 Evaluation Metrics

Rather than relying only on accuracy, the models were evaluated using:

- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**
- **ROC-AUC Score**
- **Confusion Matrix**

> **Why Recall matters?** In fraud detection, missing a fraudulent transaction is far more costly than incorrectly flagging a genuine one.

---

## 🔍 Exploratory Data Analysis

The project includes several analytical visualizations:

- Fraud vs Genuine class distribution
- Transaction amount analysis
- Time-of-day transaction trends
- SMOTE class balancing comparison
- Confusion matrices
- ROC Curve comparison
- Random Forest feature importance

---

## 💡 Key Insights

- Fraudulent transactions represent **less than 1%** of the dataset.
- SMOTE effectively balanced the training data without altering the test set.
- Random Forest achieved stronger fraud detection capability than Logistic Regression.
- Behavioral features contribute more to fraud detection than transaction amount alone.

---

## 📈 Business Recommendations

- Deploy **Random Forest** for higher fraud detection performance.
- Prioritize **Recall** to reduce undetected fraud.
- Continuously retrain the model using new transaction data.
- Combine machine learning with manual review for high-risk transactions.

---

## 📁 Project Structure

```text
DataAnalytics-L2-FraudDetection/
│
├── FraudDetection_Task3.ipynb
└── README.md
```

---

## 👩‍💻 Author

**Aparaajetha Suvarnam**

Data Analytics Intern — Oasis Infobyte (OIBSIP)

---

### ⭐ If you found this project useful, consider giving it a Star!