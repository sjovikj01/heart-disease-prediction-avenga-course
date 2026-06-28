# heart-disease-prediction-avenga-course
Final project for Data Science Course Avenga
# Heart Disease Prediction using Machine Learning

##  Project Overview

This project uses machine learning models to predict the presence of heart disease based on clinical features such as age, cholesterol, chest pain type, and heart rate.

The goal is to build a predictive system that can assist in early risk detection.

---

## Dataset

- Source: UCI Machine Learning Repository
- Dataset: Heart Disease (Cleveland)
- Samples: ~300 patients
- Target: Presence or absence of heart disease

---

##  Methods Used

### Exploratory Data Analysis (EDA)
- Distribution analysis
- Correlation analysis
- Clinical feature grouping (age, sex, cholesterol)

### Machine Learning Models
- Logistic Regression (baseline + optimized)
- Neural Network (MLPClassifier)
- SMOTE oversampling (experiment)
- Random Forest (optional benchmark)

---

##  Model Performance

| Model | Accuracy | ROC-AUC |
|------|---------|---------|
| Logistic Regression (Optimized) | 0.869 | 0.957 |
| Neural Network | ~0.86 | - |
| SMOTE Logistic Regression | 0.869 | 0.953 |

---

## Key Findings

- Logistic Regression performed best overall
- SMOTE did not improve performance due to balanced dataset
- Neural Network did not significantly outperform simpler models
- False negatives were minimized (~2 cases)

---

##  Clinical Insight

The best model achieved:
- High recall (~93%)
- Low false negatives
- Strong ROC-AUC performance

This makes it suitable as a **screening support tool**, not a medical diagnostic system.

---

## How to Run

```bash
pip install -r requirements.txt

## Dataset

This project uses the **UCI Heart Disease Dataset (Cleveland)**.

Dataset source:
https://archive.ics.uci.edu/dataset/45/heart+disease

The dataset can be downloaded directly from the UCI Machine Learning Repository.
