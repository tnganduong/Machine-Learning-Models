# Online Payment Fraud Detection System

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

An end-to-end Machine Learning project that analyzes over **6.3 million financial transactions** to accurately detect fraudulent activities in online payment systems using Machine Learning algorithms.

---

## Executive Summary

Financial fraud in digital payments leads to massive capital losses for payment providers annually. The primary challenge in fraud detection is the **extreme class imbalance** (fraudulent transactions make up less than **0.13%** of total data) and the need for **real-time scalability**.

This project provides an end-to-end solution including:
1. Custom automated Exploratory Data Analysis (EDA) pipelines for massive datasets.
2. Comparative analysis of Classical & Tree-based Machine Learning models.
3. Evaluation focused on cost-sensitive metrics (Recall, Precision, and ROC-AUC) to minimize False Negatives (uncaught frauds).

---

## Methodology
1. **Automated EDA Framework:** Developed a reusable Python function `explore_eda()` to check missing values, data distributions, statistics, and cardinality across millions of records in a single call.
2. **Data Cleaning & Validation:** Verified zero missing values across all 11 columns; identified continuous numerical variables vs. categorical types.
3. **Model Selection & Training:** Benchmark performance of traditional classifiers against tree-based structures to balance accuracy and operational speed.

---

## Key Metrics

In fraud detection:
- **Recall (Sensitivity)** is prioritized to catch as many fraudulent cases as possible (reducing **False Negatives**).
- **Precision** is balanced to avoid excessive false alarms on legitimate users (reducing **False Positives**).

---

## Tech Stack

- **Language:** Python 3.x
- **Data Manipulation & Analysis:** `pandas`, `numpy` (Handled 6.3M+ rows efficiently in memory)
- **Data Visualization:** `matplotlib`, `seaborn`
- **Machine Learning & Evaluation:** `scikit-learn`
  - *Models Used:* Logistic Regression, Decision Tree Classifier, Gaussian Naive Bayes.
  - *Preprocessing & Scaling:* `StandardScaler`, `train_test_split`.
  - *Metrics:* Confusion Matrix, Precision, Recall, F1-Score, ROC-AUC, Classification Report.

---

## Usage

1. Clone the repository
2. Follow the file source to get the link to dataset on Kaggle
3. Run the Jupyter Notebook `online_payments_fraud_detection.ipynb` to follow the steps of data preprocessing, model training, and evaluation
4. Once the model is trained and evaluated, deploy it in real-time for online payments fraud detection
