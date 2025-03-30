# **Fraud Detection in Financial Transactions**

# 📌 **Project Overview**

This project focuses on detecting fraudulent financial transactions using machine learning techniques. The dataset contains anonymized transaction details and a binary classification target (fraud or non-fraud). The goal is to build an effective predictive model to identify fraudulent transactions while handling class imbalance.

# 📂 **Dataset**
The dataset used is creditcard.csv, which consists of:

**Features**: 28 numerical variables (V1 to V28) obtained from PCA transformation, along with Time and Amount.
**Target Variable**: Class (0 = Non-Fraud, 1 = Fraud).
**Imbalance**: The dataset is highly imbalanced, with fraudulent transactions being a small percentage of the total.

# 🏗 **Model Training & Evaluation**

**1. Data Preprocessing**
**Train-Test Split**: 90% training, 10% testing (stratified sampling).
**Feature Scaling**: Standardized using StandardScaler.
**Class Balancing**: SMOTE (Synthetic Minority Over-sampling) is applied to handle the class imbalance.

**2. Model Selection**
**Algorithm Used**: Random Forest Classifier
**Hyperparameters:**
n_estimators=100
random_state=42

**3. Model Evaluation**
**Confusion Matrix**: Visualizes TP, FP, TN, FN
**Metrics:**
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC Score

# 📊 **Visualization**
Confusion Matrix Heatmap (using seaborn)

# 🏆 **Conclusion**
This project successfully implements a fraud detection system using Random Forest, with SMOTE to handle class imbalance. Further refinements can improve precision and recall for fraud detection.
