# 📊 Customer Monthly Charges Prediction (ML Project)

## 🚀 Overview

This project focuses on predicting **monthly charges of telecom customers** using Machine Learning.
It demonstrates how **feature engineering and proper data preprocessing** can significantly improve model performance.

---

## 🎯 Objective

To build a regression model that accurately predicts **Monthly Charges** based on customer attributes and analyze the key factors influencing billing.

---

## 📂 Dataset

* Telecom Customer Dataset
* Includes customer details such as tenure, billing, contract type, and services

---

## ⚙️ Workflow

### 🔹 1. Data Preprocessing

* Cleaned column names
* Converted `TotalCharges` to numeric (handled invalid values)
* Removed missing data
* Encoded categorical features using One-Hot Encoding

---

### 🔹 2. Exploratory Data Analysis (EDA)

* Analyzed relationships between features
* Visualized:

  * Tenure vs Monthly Charges
  * Correlation between numerical features

---

### 🔹 3. Feature Engineering

Initial model used:

* `tenure`
* `TotalCharges`

Improved model added:

* `Contract`
* `InternetService`

👉 This significantly enhanced predictive performance.

---

### 🔹 4. Models Used

* Linear Regression
* Ridge Regression

---

### 🔹 5. Model Evaluation Metrics

* Mean Squared Error (MSE)
* R² Score

---

## 📈 Results

### 🔸 Initial Model (Basic Features)

* **R² Score:** ~0.70
* **MSE:** ~271

### 🔸 Improved Model (Feature Engineered)

* **R² Score:** **0.91**
* **MSE:** **78.64**

---

## 📊 Visualization

### 🔹 Actual vs Predicted (Improved Model)

This plot compares predicted values with actual values along with an ideal prediction line.

> The closer the points are to the red line, the better the model performance.


<img width="1715" height="1361" alt="image" src="https://github.com/user-attachments/assets/6a0efc4b-310c-4ae8-b7fe-5a4eefc638e4" />


## 🔍 Key Insights

* **Contract type** and **Internet service** are strong predictors of monthly charges
* Feature engineering improved model performance significantly (R²: 0.70 → 0.91)
* Minimal difference between Linear and Ridge regression indicates:

  * Low overfitting
  * Well-structured dataset

---

## 🧠 Model Comparison

* Linear Regression R²: **0.9126**
* Ridge Regression R²: **0.9126**

👉 Regularization had minimal impact due to the simplicity and quality of features.

---

## 🛠️ Tech Stack

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib

---

## ▶️ How to Run

```bash
pip install -r requirements.txt
jupyter notebook
```

---

## 📌 Future Improvements

* Add more features (Payment Method, Customer Demographics)
* Try advanced models (Random Forest, Gradient Boosting)
* Hyperparameter tuning
* Deploy as a web app using Streamlit

---


---

## 💡 Key Takeaway

This project highlights that **feature engineering plays a more critical role than model complexity** in achieving high performance in machine learning tasks.

