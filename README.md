# investment-classification-recommender
Machine learning models to classify investment propensities and recommend financial products for banking clients.


# 🧠 Investment Classification & Recommendation System

This project applies machine learning techniques to classify 5000 bank clients based on their **income** and **accumulation investment** propensities. Based on the classification, a simple rule-based recommendation system assigns personalized financial products.

## 📌 Problem Statement

Banks and fintech platforms often need to understand clients' investment behavior to personalize offerings. This project builds models to classify clients and recommend suitable financial products.

---

## 🛠️ Features

- Binary classification for **IncomeInvestment** and **AccumulationInvestment**
- Supervised models: Logistic Regression, AdaBoost (with Perceptron and Decision Trees), Random Forest
- Model evaluation using accuracy, precision, recall, and F1-score
- Rule-based recommendation engine using predicted labels and client risk profiles

---

## 📊 Results

### 🟩 Best Performing Model: Random Forest

| Target                         | Accuracy | Precision | Recall | F1-Score |
|-------------------------------|----------|-----------|--------|----------|
| Income Investment Propensity  | 0.825    | 0.890     | 0.607  | 0.722    |
| Accumulation Investment       | 0.831    | 0.919     | 0.735  | 0.817    |

- Best Hyperparameters for Income:
  - `max_depth=12`, `n_estimators=125`, `min_samples_split=6`
- Best Hyperparameters for Accumulation:
  - `max_depth=10`, `n_estimators=125`, `min_samples_split=10`

---

### ⚖️ Model Comparison

| Model                      | Income F1 | Accum. F1 |
|---------------------------|-----------|-----------|
| Random Forest             | **0.722** | **0.817** |
| AdaBoost (Decision Trees) | 0.679     | 0.767     |
| AdaBoost (Perceptron)     | 0.623     | 0.625     |
| Logistic Regression (v2)  | 0.672     | 0.677     |


