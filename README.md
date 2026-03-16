# 🏦 Bank Customer Churn Prediction: An End-to-End ML Solution

![Python](https://img.shields.io/badge/Python-3.14-blue.svg)
![XGBoost](https://img.shields.io/badge/XGBoost-Advanced-red.svg)
![Imbalanced Data](https://img.shields.io/badge/SMOTE-Imbalanced_Data-orange.svg)

## 📑 Table of Contents
- [Introduction](#-introduction)
- [List of Features](#-list-of-features)
- [Technologies Used](#-technologies-used)
- [What I Learned & Accomplished](#-what-i-learned--accomplished)
- [PhuocCaoData](#-PhuocCaoData)
- [Examples](#-examples)
- [Acknowledgments](#-acknowledgments)

## 🌟 Introduction
Customer attrition (churn) is one of the most significant hidden costs for financial institutions. This project is a complete Machine Learning pipeline designed to predict credit card customer churn based on a dataset of 10,127 records.

**Why was this project built?**
While many beginner projects chase misleading "Accuracy" metrics on highly imbalanced datasets, this project was built to solve a real-world business problem. It focuses strictly on optimizing **Recall** and translating model predictions into actionable Business ROI. By accurately identifying at-risk customers, this solution enables targeted retention campaigns that can potentially save the bank an estimated **$1.75M annually**.

## ✨ List of Features
- **Zero Data Leakage:** Strict Train/Test splitting *before* applying techniques like SMOTE and Bayesian Target Encoding.
- **Business-Centric Evaluation:** Prioritizes Recall (>91%) and PR-AUC over standard Accuracy to effectively capture churning customers.
- **Actionable CRM Framework:** Outputs probability scores that categorize customers into 4 distinct Risk Tiers (Critical, High, Medium, Low) for tailored Customer Service strategies.
- **Interactive Visualizations:** Utilizes Plotly for interactive feature importance and Seaborn/Matplotlib for presentation-ready Exploratory Data Analysis (EDA).

## 💻 Technologies Used
- **Language:** Python 3.14
- **Data Manipulation:** `pandas`, `numpy`
- **Machine Learning:** `scikit-learn`, `xgboost`, `imbalanced-learn` (SMOTE), `category_encoders`
- **Visualization:** `matplotlib`, `seaborn`, `plotly`
- **Environment:** Jupyter Notebook / VS Code

## 🧠 What I Learned & Accomplished
Throughout this project, I transitioned from simply "running machine learning models" to solving a tangible business problem. Here are my key takeaways:

- **Business Integration:** I learned how to translate technical metrics into actionable business language. Instead of stopping at model evaluation, I estimated a potential **$1.75M annual saving** and designed a practical 4-tier CRM risk framework for stakeholders.
- **Preventing Data Leakage:** I mastered the rigorous sequence of data preprocessing. I now fully understand why techniques like **SMOTE** and **Bayesian Target Encoding** must strictly be applied *after* the train/test split to prevent synthetic data from polluting the validation metrics.
- **Beyond the "Accuracy" Trap:** I realized that "Accuracy" is a highly misleading metric for imbalanced datasets (16% churn rate). I successfully prioritized and optimized the XGBoost model for **Recall (capturing >91% of churners)** and Precision-Recall AUC.
- **Explainable AI (XAI):** I utilized Feature Importance to understand the *why* behind the model's predictions, proving that customer behavioral data (transaction frequency/amounts) heavily outweighs demographic data (age/gender) in predicting churn.

## 🚀 PhuocCaoData

**1. Clone the repository & Setup Environment:**

** Create and activate virtual environment (Windows)
python -m venv churn_env
churn_env\Scripts\activate

** Install dependencies
pip install pandas numpy matplotlib seaborn plotly scikit-learn xgboost imbalanced-learn category_encoders

**2. Run the project:**
*Ensure the raw dataset BankChurners.csv is located in the root directory.
*Open the main analysis notebook:
jupyter notebook BankChurners_Churn_Prediction_1.ipynb

## 📊 Examples

1. Identifying Key Churn Drivers
The model reveals that behavioral metrics (e.g., total transaction count and amount) are far more critical than demographic data (Age/Gender).

2. Actionable Output (Risk Tiers)
Instead of a simple 0 or 1 output, the model provides a strategic action plan. Here is an example of how the output is categorized for the business team:
🔴 Critical (>80% risk): Immediate human outreach required.
🟠 High (60–80% risk): Automated retention campaign enrollment.
🟡 Medium (30–60% risk): Monitor closely for the next 30 days.
🟢 Low (<30% risk): Standard customer journey.

## 🙏 Acknowledgments

Dataset provided by the open-source community (Credit Card Customers dataset).

Formatting inspiration drawn from standard open-source documentation practices and tools like readme.so.

