# 🕵️‍♂️ Fraud Detection in Financial Transactions

## 📌 Overview

This project focuses on detecting **fraudulent banking transactions** using machine learning. Built as a simulation of real-world financial data, the project leverages EDA, logistic regression, and a web-based Streamlit interface to predict fraud in user-submitted transactions.

---

## ⚙️ Tech Stack

- **Python Version:** 3.9.6 (recommended for compatibility)
- **Environment:** Jupyter Notebook + Streamlit + Conda
- **Libraries Used:**
  - `pandas`, `numpy`
  - `matplotlib`, `seaborn`
  - `scikit-learn`
  - `joblib`
  - `streamlit`

---

## 🧪 Notebooks & Model Training

Notebook: `analysis_fraud.ipynb`

📦 Download the dataset [here](https://drive.google.com/file/d/1d-ojJ5jn-6hH3duF54wUhiFh0sfWNtKW/view?usp=sharing)
### Key steps:
- Load dataset `AIML Dataset.csv`
- Perform EDA (visualizations, correlation, class imbalance)
- Feature engineering (e.g., `balanceDiffOrg`, `balanceDiffDest`)
- Drop irrelevant features (`step`, `nameOrig`, `nameDest`, etc.)
- Train a logistic regression model using `Pipeline` and `ColumnTransformer`
- Save trained model using `joblib`

### Model Performance:
- **Accuracy:** 94.53%
- **Recall (fraud):** 93%
- **Precision (fraud):** ~2%

---

## 📱 Web App with Streamlit

Streamlit interface is implemented in `fraud_detection.py` to allow users to manually input transaction details and predict fraud in real-time.

### 📦 How to run:

```bash
# Make sure to activate your Conda environment with Python 3.9.6
streamlit run fraud_detection.py
