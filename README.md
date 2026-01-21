# Fraud Detection Model

## 📌 Overview
This repository contains an end-to-end fraud detection machine learning pipeline.  
The project focuses on handling **highly imbalanced transaction data** and provides a reproducible workflow from data ingestion to model evaluation.

The model is designed for **decision support**, prioritizing fraud detection performance over raw accuracy.

---

## 🧠 Problem Context
Fraudulent transactions typically represent a very small portion of total transactions (≈3–5%).  
As a result:
- Accuracy is misleading
- Missing fraud (false negatives) is costly
- Recall and F1-score are more meaningful evaluation metrics

---

## 🗂️ Data Source
- Kaggle dataset (IEEE-CIS fraud detection):https://www.kaggle.com/datasets/lnasiri007/ieeecis-fraud-detection/data
- Only train_identity and train_transaction used for training model.

### Dataset Description
- Transaction-level tabular dataset
- Mix of numerical and optional categorical features
- Binary target variable:
  - `0` → Non-fraud
  - `1` → Fraud

> ⚠️ The original dataset is **not included** in this repository due to privacy and confidentiality constraints.



## 🛠️ Libraries & Dependencies

### Core Requirements
- Python
- pandas
- numpy
- scikit-learn
- xgboost
- joblib

### Optional (EDA / Visualization)
- matplotlib
- seaborn
- jupyter

## 🚀 Getting Started


### Step 1: Clone the repository

```bash
git clone https://github.com/aitechinstitute/ab-25-06-beginner-ai.git
cd ab-25-06-beginner-ai
```
### Step 2: Download data from kaggle

Datasets are not able to load into Github due to the size, please use the link below to download train_transactions.csv and train_identity.csv fro Kaggle. Then save them in the same location with project to run.
https://www.kaggle.com/datasets/lnasiri007/ieeecis-fraud-detection/data

### Step 3: Launch Jupyter Lab (or VS Code) to open project

```bash
jupyter lab
```
---

## Assumptions & Limitations

- Dataset contains limited fraud examples, restricting recall performance

- Model performance depends heavily on feature quality

- Hardware restrictions required reducing dataset size and narrowing hyperparameter search ranges.

## Next Steps

### 1. Stakeholder Presentation: 
    Share findings with stakeholders to secure investment in upgraded computational resources and expanded datasets.

### 2. Model Deployment: 
    Integrate the fraud detection model into the bank’s application with real-time notification systems for suspicious activity.

### 3. Performance Monitoring: 
    Establish weekly reviews of recall and F1 scores to track improvements, identify weaknesses, and refine the model continuously.
