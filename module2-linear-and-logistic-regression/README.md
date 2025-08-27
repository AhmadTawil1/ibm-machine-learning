# 📘 Module 2: Regression Models (IBM Machine Learning Course)

This module covers **supervised regression methods** — from linear models to logistic regression — and introduces optimization techniques like gradient descent. The work includes theory, examples, and a practical lab implementation (`Logistic_Regression.ipynb`).

---

## 📂 Contents
- Linear Regression
- Multiple Linear Regression
- Polynomial Regression
- Nonlinear Regression
- Logistic Regression
- Training Logistic Regression with Gradient Descent & SGD
- Lab: `Logistic_Regression.ipynb`

---

## 🧠 Key Concepts

### 🔹 Linear Regression
- Predicts continuous outcomes with a straight line.  
- Formula:  
  `ŷ = θ₀ + θ₁x`  
- Cost function: **Mean Squared Error (MSE)**.

### 🔹 Multiple Linear Regression
- Extends to multiple predictors.  
- Formula:  
  `ŷ = θ₀ + θ₁x₁ + θ₂x₂ + … + θₙxₙ`.

### 🔹 Polynomial Regression
- Models curved relationships with polynomial terms.  
- Solved via linear regression on transformed features.  
- Risk: **overfitting** with high-degree polynomials.

### 🔹 Nonlinear Regression
- Models non-polynomial relationships (exponential, logarithmic, sinusoidal).  
- Examples: GDP growth (exponential), diminishing returns (logarithmic).

### 🔹 Logistic Regression
- Binary classification (0/1).  
- Outputs probabilities via **sigmoid function**:  
  `σ(z) = 1 / (1 + e⁻ᶻ)`  
  where `z = θ₀ + θ₁x₁ + … + θₙxₙ`.  
- Cost function: **Log Loss**.  
- Uses a threshold (commonly 0.5) to assign classes.

### 🔹 Training (Gradient Descent & SGD)
- Iterative optimization to minimize cost functions.  
- **Gradient Descent**: full dataset each update (slower, stable).  
- **Stochastic Gradient Descent (SGD)**: random subset each update (faster, noisier).  
- Learning rate controls step size.  

---

## 🧩 Lab Summary (`Logistic_Regression.ipynb`)
- Implemented logistic regression for binary classification.  
- Preprocessing: feature handling, target encoding.  
- Trained using gradient descent.  
- Evaluated using accuracy and log loss.  
- Compared how gradient descent vs. stochastic gradient descent affect convergence.  

---

## 📊 Skills Learned
- Building regression models for linear, nonlinear, and binary classification tasks.
- Understanding polynomial feature transformations.
- Implementing and interpreting logistic regression.
- Training models using gradient descent & SGD.
- Evaluating models with log loss and classification accuracy.
- Recognizing and addressing **overfitting vs. generalization**.

---

## 🚀 Next Steps (Module 3 Preview)
- Classification metrics (accuracy, precision, recall, F1 score).
- Multi-class classification methods.
- Decision Trees, Random Forests, and SVMs.
