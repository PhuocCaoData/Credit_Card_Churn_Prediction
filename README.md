# Credit_Card_Churn_Prediction
An end-to-end ML pipeline using XGBoost to predict bank customer churn. Focuses on handling imbalanced data, high Recall, and actionable business ROI. 🏦📊

# 🏦 Bank Customer Churn Prediction: An End-to-End ML Solution

![Python](https://img.shields.io/badge/Python-3.14-blue.svg)
![XGBoost](https://img.shields.io/badge/XGBoost-Advanced-red.svg)
![Imbalanced Data](https://img.shields.io/badge/SMOTE-Imbalanced_Data-orange.svg)

## 📑 Table of Contents
- [Introduction](#-introduction)
- [List of Features](#-list-of-features)
- [Technologies Used](#-technologies-used)
- [Install](#-install)
- [Use](#-use)
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

## 🛠️ Install
To get a local copy up and running, follow these simple steps:

