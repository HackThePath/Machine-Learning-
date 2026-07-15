# 💳 Credit Card Fraud Detection using Machine Learning

![Credit card](https://github.com/HackThePath/Machine-Learning-/blob/ffd318ed88c894d3d875ac96d4deaaac5d1ba354/Credit-Card-Fraud-Detection/img.png)

> Detecting fraudulent credit card transactions using machine learning to help financial institutions reduce financial losses and improve transaction security.

---

## 📌 Project Overview

Credit card fraud has become one of the biggest challenges faced by banks and financial institutions. Millions of transactions are processed every day, making it impossible to manually inspect every transaction for fraudulent activity.

This project focuses on building an intelligent machine learning solution capable of distinguishing between legitimate and fraudulent credit card transactions based on historical transaction data.

Using supervised machine learning techniques, the project compares multiple classification algorithms and identifies the best-performing model for fraud detection through evaluation and hyperparameter tuning.

---

## 🎯 Problem Statement

Financial institutions lose billions of dollars every year due to fraudulent credit card transactions.

The challenge lies in accurately identifying fraudulent transactions because fraud cases represent only a very small percentage of the total transactions.

The objective of this project is to build a machine learning model that can accurately detect fraudulent transactions while minimising false alarms and missed fraud cases.

---

## 💼 Business Objective

The primary goals of this project are to:

* Detect suspicious credit card transactions automatically.
* Reduce financial losses caused by fraudulent activities.
* Assist fraud investigation teams by identifying high-risk transactions.
* Improve transaction monitoring through machine learning.
* Compare multiple classification models and select the most suitable model for fraud detection.

---

## 📊 Dataset Information

The project uses the **Credit Card Fraud Detection** dataset containing real-world anonymised credit card transactions.

### Dataset Summary

* Total Transactions: **284,807**
* Fraudulent Transactions: **492**
* Legitimate Transactions: **284,315**
* Features: **31**

### Dataset Features

* **Time** – Time elapsed between each transaction and the first transaction in the dataset.
* **V1 – V28** – Anonymised numerical features obtained using Principal Component Analysis (PCA).
* **Amount** – Transaction amount.
* **Class** – Target variable.

  * `0` → Legitimate Transaction
  * `1` → Fraudulent Transaction

---

## ⚠️ Project Challenge

The dataset is **highly imbalanced**.

Approximately:

* **99.8%** Legitimate Transactions
* **0.2%** Fraudulent Transactions

Because of this imbalance, model performance cannot be evaluated using accuracy alone.

Greater emphasis is placed on:

* Precision
* Recall
* F1 Score
* ROC-AUC Score
* Confusion Matrix

---

# 🛠️ Project Workflow

```text
Dataset Collection
        │
        ▼
Data Understanding
        │
        ▼
Data Preprocessing
(Missing Values • Duplicate Removal)
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Feature Engineering
        │
        ▼
Train-Test Split
        │
        ▼
Feature Scaling
        │
        ▼
Model Building
│
├── Logistic Regression
├── Decision Tree
└── Random Forest
        │
        ▼
Model Evaluation
        │
        ▼
Hyperparameter Tuning
(GridSearchCV)
        │
        ▼
Final Model Selection
```

---

# ⚙️ Data Preprocessing

The following preprocessing techniques were performed:

* Missing value analysis
* Duplicate transaction removal
* Class distribution analysis
* Feature engineering
* Feature scaling using StandardScaler
* Train-test split with stratified sampling

---

# 📈 Exploratory Data Analysis

The dataset was explored to understand transaction behaviour and class distribution.

The analysis included:

* Dataset structure
* Statistical summary
* Missing value analysis
* Duplicate detection
* Class imbalance analysis
* Transaction amount distribution
* Fraud vs legitimate transaction comparison

---

# 🤖 Machine Learning Models

Three supervised machine learning classification models were developed and compared.

### Logistic Regression

A simple baseline model used for binary classification.

### Decision Tree

A tree-based model capable of learning nonlinear decision boundaries.

### Random Forest

An ensemble learning algorithm combining multiple decision trees to improve prediction accuracy and reduce overfitting.

---

# 📊 Model Evaluation

The models were evaluated using the following performance metrics:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC Score
* Confusion Matrix

Since the dataset is highly imbalanced, Recall and F1 Score were considered more informative than Accuracy when comparing model performance.

---

# 🎯 Hyperparameter Tuning

The Random Forest model was further optimised using **GridSearchCV** with cross-validation.

Different combinations of hyperparameters such as:

* Number of Trees
* Maximum Tree Depth
* Minimum Samples Split

were evaluated to identify the best-performing configuration.

---

# 🧰 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook
* Joblib

---

# 📁 Project Structure

```text
Credit_Card_Fraud_Detection/
│
├── creditcard.csv
├── Credit_Card_Fraud_Detection.ipynb
├── credit_card_fraud_model.pkl
├── credit_card_scaler.pkl
├── README.md
└── images/
```

---

# 🚀 Key Learning Outcomes

Through this project, I gained practical experience in:

* Data preprocessing for machine learning
* Handling highly imbalanced datasets
* Feature engineering
* Building supervised classification models
* Comparing machine learning algorithms
* Hyperparameter tuning using GridSearchCV
* Evaluating classification models using business-focused metrics
* Interpreting model performance for real-world fraud detection

---

# 📌 Future Improvements

Possible enhancements to this project include:

* Applying advanced imbalance-handling techniques such as SMOTE.
* Exploring Gradient Boosting algorithms like XGBoost and LightGBM.
* Developing a real-time fraud prediction web application using Streamlit or Flask.
* Deploying the trained model as a REST API for real-world integration.

---

# ⭐ Conclusion

This project demonstrates an end-to-end machine learning workflow for credit card fraud detection, beginning with raw transaction data and progressing through preprocessing, feature engineering, model development, evaluation and optimisation.

By comparing multiple machine learning algorithms and selecting the best-performing model through systematic evaluation, the project highlights how data-driven solutions can support financial institutions in detecting fraudulent transactions more effectively and improving transaction security.

