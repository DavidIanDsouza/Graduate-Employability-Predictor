# 🎓 Graduate Employability Predictor

## By: Anish, David, Rahul, Sean, and Timur

## 🌟 Introduction

This project investigates and compares three distinct machine learning models, **Logistic Regression**, **Decision Trees**, and a **Neural Network**, for the critical task of **predicting graduate employability**.

By implementing and rigorously evaluating their performance metrics (including Accuracy, Recall, and F1-Score) on a standardized dataset, we aim to identify the most effective and robust model for this binary classification challenge.

---

## 💾 Dataset and Preprocessing

The analysis uses the `CollegePlacement.csv` dataset. Key steps in data preparation included:

* **Feature Removal:** The irrelevant `College_ID` column was dropped.
* **Encoding:** Categorical fields (`Internship_Experience`, `Placement`) were converted to numerical `1`/`0` values.
* **Scaling:** All numerical features were scaled using **`StandardScaler`** to ensure consistent range.
* **Splitting:** The final dataset was split into an **80% training set** (8000 samples) and a **20% testing set** (2000 samples).

### Data Imbalance

Exploratory analysis showed a significant class imbalance:
* **No Placement:** 83.41%
* **Yes Placement:** 16.59%

This imbalance makes **Recall** (correctly identifying the placed students) a crucial metric for evaluating model success.

---

## 📊 Model Performance Comparison

Three models were trained and evaluated on the test set. The results demonstrate clear differences in predictive power:

| Metric | Logistic Regression (LR) | Decision Tree (DT) | Neural Network (NN) |
| :--- | :--- | :--- | :--- |
| **Accuracy** | 0.9035 | 0.9630 | **0.9930** |
| **Recall** | 0.6074 | 0.9417 | **0.9847** |
| **F1-Score** | 0.6723 | 0.8924 | **0.9787** |

