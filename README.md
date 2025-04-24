# 💳 Credit Card Fraud Detection

![Credit Card Fraud Detection](images/credit-card.jpg)
This project develops a classification model to detect fraudulent credit card transactions using anonymized transaction data. The model aims to reduce false positives while maintaining high detection accuracy in a highly imbalanced dataset.

---

## 📊 Problem Statement

Credit card fraud is a major concern for banks and consumers. Our goal is to build a machine learning model that:
- Detects fraudulent transactions accurately.
- Minimizes false positives (non-fraud classified as fraud).
- Handles class imbalance using data sampling techniques.
- Uses domain-inspired feature engineering like transaction patterns and location mismatches.

---

## 📁 Project Structure

Credit-Card-Fraud-Detection/ │ ├── data/ # Dataset (creditcard.csv) ├── notebooks/ │ └── Model_Final.ipynb # Main model development notebook ├── PyOD/ # Anomaly detection methods ├── images/ # Visualizations used in EDA ├── src/ # Utility scripts (optional) ├── fraud_credit.py # Python script version ├── requirements.txt └── README.md


---

## 📥 Dataset

- Download from [Kaggle – Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- Place `creditcard.csv` inside the `data/` folder.

---

## ⚙️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/Credit-Card-Fraud-Detection.git
   cd Credit-Card-Fraud-Detection

## ⚙️Install dependencies
- pip install -r requirements.-txt
- jupyter notebook

## 🧠 Features & Engineering
Transaction Amount

Timestamp-derived features (hour, day)

Spending Patterns (e.g., frequency in last X minutes)

Location Mismatch (if merchant/user zip codes differ)

Transaction Type, Device Info (if available)

## ⚖️ Class Imbalance Handling
SMOTE (Synthetic Minority Oversampling Technique)

Random Undersampling

Combination Techniques

Anomaly Detection using PyOD

## 🧪 Model Evaluation
Confusion Matrix

ROC-AUC Score

Precision, Recall, F1-Score

PR Curve (Precision-Recall)

We aim for high recall (catch all frauds) while controlling precision (don’t misclassify genuine users).

## 🤖 Models Used
Logistic Regression

Decision Trees & Random Forest

XGBoost

LightGBM

PyOD Ensemble (for anomaly detection)

## 📈 Results
High AUC and Recall achieved with balanced SMOTE + LightGBM.

Significantly improved fraud catch rate compared to baseline.

## 🧾 How to Run the Code
Open Model_Final.ipynb for full training pipeline.

Run fraud_credit.py if you prefer a Python script version.

All visualizations are inside images/.

##  🙌 Acknowledgments
Kaggle Credit Card Fraud Dataset

Scikit-learn, imbalanced-learn, PyOD, XGBoost, LightGBM


