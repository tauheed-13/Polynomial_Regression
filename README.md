## 📖 Project Overview
This project demonstrates the implementation of **Simple Linear Regression** and **Polynomial Regression** using the **Scikit-learn** library and compares their performance on a **non-linear dataset**.

The objective of this project is to:
- Understand why Simple Linear Regression fails on non-linear data
- Learn how Polynomial Regression improves predictions
- Explain why Polynomial Regression is still a Linear Regression model
- Understand the importance of selecting the correct polynomial degree

---

## 🔹 Simple Linear Regression
Simple Linear Regression models the relationship between an input variable `X` and an output variable `y` using a straight line.

### Mathematical Equation:
\[
y = wX + b
\]

### Key Characteristics:
- Assumes a linear relationship between input and output
- Works well for datasets with straight-line patterns
- Easy to interpret and computationally efficient

### Limitation:
For non-linear datasets, Simple Linear Regression **underfits** the data, resulting in high prediction error and poor performance.

---

## 🔹 Polynomial Regression
Polynomial Regression enhances Linear Regression by transforming the input features into polynomial features.

### Mathematical Equation:
\[
y = w_0 + w_1X + w_2X^2 + w_3X^3 + \dots + w_nX^n
\]

This allows the model to capture curved and complex relationships present in non-linear datasets.

---

## ❓ Why Polynomial Regression Is Still a Linear Model
Despite its name, Polynomial Regression is considered a **Linear Regression model** because:

- The model remains linear with respect to the parameters (weights)
- Polynomial terms (`X²`, `X³`, etc.) are treated as new features
- Linear optimization techniques are used for training

Example:
\[
y = w_0 + w_1X + w_2X^2
\]

Here, the model is linear in terms of `w₀`, `w₁`, and `w₂`.

---

## 📐 What Is Degree in Polynomial Regression?
The **degree** of a polynomial refers to the highest power of the input variable used in the model.

| Degree | Model Behavior |
|------|---------------|
| 1 | Straight line (Simple Linear Regression) |
| 2 | Parabolic curve |
| 3 | Cubic curve |
| Higher | More complex curves |

---

## ⚠️ Importance of Choosing the Right Degree

### 🔸 Low Degree (Underfitting)
- Model is too simple
- Cannot capture non-linear patterns
- High bias

### 🔸 High Degree (Overfitting)
- Model fits noise instead of actual trends
- Poor performance on unseen data
- High variance

### ✅ Optimal Degree
- Balances bias and variance
- Generalizes well to new datasets

Choosing the correct polynomial degree is crucial for achieving optimal model performance.

---

## 📊 Model Comparison

| Feature | Simple Linear Regression | Polynomial Regression |
|------|--------------------------|----------------------|
| Relationship type | Linear | Linear + Non-linear |
| Dataset suitability | Linear datasets | Non-linear datasets |
| Model complexity | Low | Controlled by degree |
| Overfitting risk | Low | High (if degree is large) |

---

## 🎯 Conclusion
- Simple Linear Regression is limited to linear data
- Polynomial Regression handles non-linear patterns effectively
- Polynomial Regression is still a Linear Regression model
- Proper degree selection is essential to avoid underfitting or overfitting

This project provides a clear understanding of when and why Polynomial Regression should be used over Simple Linear Regression.
