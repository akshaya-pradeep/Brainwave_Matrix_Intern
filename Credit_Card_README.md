# 💳 Credit Card Fraud Detection using Machine Learning

This project is part of my AI/ML Internship, where the goal is to build a fraud detection model capable of identifying fraudulent credit card transactions using supervised learning techniques and proper handling of imbalanced data.

---

## 📌 Problem Statement

Credit card fraud causes billions in losses globally. Detecting fraudulent transactions accurately, especially when the fraud-to-normal ratio is extremely imbalanced, is a key challenge. This project aims to build a model that identifies fraud effectively using machine learning.

---

## 🧠 Techniques Used

- **Data Preprocessing**
  - Handled missing values (none in this dataset)
  - Feature scaling using `StandardScaler`
- **Handling Imbalanced Data**
  - Applied **SMOTE** (Synthetic Minority Over-sampling Technique) to balance the classes
- **Supervised Machine Learning**
  - Used **Random Forest Classifier** for classification
- **Model Evaluation**
  - Confusion Matrix
  - Classification Report (Precision, Recall, F1-score)
  - **ROC AUC Score**

---

## 📂 Dataset

- **Source:** [Kaggle - Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- 284,807 transactions with 30 features:
  - `Time`, `Amount`, `V1` to `V28` (anonymized using PCA)
  - `Class`: 0 = Legitimate, 1 = Fraudulent

---

## 🔍 Evaluation Metrics

| Metric            | Value (example) |
|-------------------|-----------------|
| Accuracy          | 99.3% (not reliable for imbalance) |
| Precision (fraud) | 0.89            |
| Recall (fraud)    | 0.84            |
| ROC AUC Score     | 0.91            |

---

## 📁 Files

| File | Description |
|------|-------------|
| `fraud_detection.ipynb` | Main notebook with complete training pipeline |
| `model.pkl`             | Saved Random Forest model |
| `scaler.pkl`            | Saved StandardScaler used for prediction |
| `README.md`             | Project overview and guide |
| `creditcard.csv`        | Raw dataset (not included in repo due to size) |
