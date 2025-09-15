# Subscription Banking - Predictive Modeling

![Notebook](https://img.shields.io/badge/Notebook-Python-blue) ![Kaggle](https://img.shields.io/badge/Kaggle-Playground-orange)

This repository contains a Jupyter Notebook for the **Subscription Banking Prediction** task from the [Kaggle Playground Series S5E8](https://www.kaggle.com/competitions/playground-series-s5e8/overview). The goal is to predict customer subscription behavior based on their historical and demographic data.  

---

## 📌 Overview

In this competition, the challenge is to **predict which customers will subscribe** to a banking service. The dataset contains anonymized customer information, including demographic features, historical interactions, and subscription history. The target variable is binary, indicating whether a customer subscribed (`1`) or not (`0`).  

---

## 🛠️ Data

The dataset used in this notebook includes:

- **Train data**: Features and target labels for training models.  
- **Test data**: Features without target labels, used for making predictions.  

> **Link to competition and dataset:** [Kaggle Playground Series S5E8](https://www.kaggle.com/competitions/playground-series-s5e8/overview)  

---

## 🔍 Data Preprocessing

The following preprocessing steps were applied:

1. **Handling Missing Values**  
   - Missing values were imputed using mean/mode depending on feature type.  

2. **Categorical Encoding**  
   - One-Hot , Label, Ordinal Encodings were used based on feature type nominal or ordinal.

3. **Feature Scaling**  
   - StandardScaler, RobustScaler were applied to numerical features to normalize distributions.  

4. **Balancing Data**  
   - Class weights were used.


---

## 🏗️ Modeling

The notebook implements multiple classification models:

- Logistic Regression  
- Random Forest Classifier  
- XGBoost Classifier  
- Stacking Algorithm (Base Learners -> XGBoost, RFClassifier, Meta Learners -> Logistic Regression)

The models were evaluated using:

- **Accuracy**  
- **AUC-ROC Score** (main evaluation metric)  
- Cross-validation for robust performance estimation  

---

## 📊 Visualization

- ROC curves and AUC scores were visualized to compare model performance.  

---

