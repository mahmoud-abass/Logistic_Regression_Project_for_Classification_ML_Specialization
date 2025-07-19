# 🚀 Logistic Regression for Classification

A from-scratch implementation of **Logistic Regression** and **Regularized Logistic Regression** for practical **binary classification**, with clear **visualizations, clean code, and mathematical explanations** to build strong foundational understanding.

---

## ✨ Overview

This project covers:

✅ Logistic Regression to predict **student admission** based on exam scores.  
✅ Regularized Logistic Regression for **microchip quality classification** with non-linear boundaries using polynomial features.  
✅ Visualizing datasets, decision boundaries, and training progress.  
✅ Building intuition for sigmoid, cost, gradient computation, and regularization.

---

## 📊 Dataset

**Part 1: Student Admission Prediction**  
- Features: `Exam 1`, `Exam 2` scores.  
- Target: `0` = Not Admitted, `1` = Admitted.

**Part 2: Microchip Quality Classification**  
- Features: `Test 1`, `Test 2` results.  
- Target: `0` = Rejected, `1` = Accepted.

---

## 🛠️ Methods

- **Logistic Regression**: Implements sigmoid, cross-entropy cost, gradient computation, and gradient descent optimization.
- **Regularized Logistic Regression**: Adds **L2 regularization** and **polynomial feature mapping** to handle non-linear boundaries.
- **Visualization**: Uses Matplotlib for clear data and boundary plots.
- **Evaluation**: Calculates accuracy on training data for performance validation.

---

## 🪐 Mathematical Foundations

### 1️⃣ Logistic Regression

Predicts the probability of class `1` using:

\[
f_{w,b}(x) = \frac{1}{1 + e^{-(w \cdot x + b)}}
\]

**Cost Function:**

\[
J(w,b) = -\frac{1}{m} \sum_{i=1}^m [ y^{(i)} \log(f_{w,b}(x^{(i)})) + (1 - y^{(i)}) \log(1 - f_{w,b}(x^{(i)})) ]
\]

**Gradient:**

\[
\frac{\partial J}{\partial w_j} = \frac{1}{m} \sum_{i=1}^m (f_{w,b}(x^{(i)}) - y^{(i)}) x_j^{(i)}
\]
\[
\frac{\partial J}{\partial b} = \frac{1}{m} \sum_{i=1}^m (f_{w,b}(x^{(i)}) - y^{(i)})
\]

---

### 2️⃣ Regularized Logistic Regression

Adds **L2 regularization** to penalize large weights:

\[
J_{reg}(w,b) = J(w,b) + \frac{\lambda}{2m} \sum_{j=1}^n w_j^2
\]

Regularized gradients:

\[
\frac{\partial J_{reg}}{\partial w_j} = \frac{\partial J}{\partial w_j} + \frac{\lambda}{m} w_j
\]

---

## 🎯 Results

✅ **Part 1 (Student Admission):**  
Achieved **~89% accuracy** with a **linear decision boundary**.

✅ **Part 2 (Microchip Classification):**  
Achieved **~82% accuracy** with a **non-linear decision boundary** using polynomial feature mapping and regularization.

✅ All results visualized with clear plots of **data points, decision boundaries, and cost convergence** for transparent analysis.

---

## 📂 Project Structure

```
📁 logistic-regression-classification/
│
├── logistic_regression_project.ipynb   # Full step-by-step notebook
├── data/
│   ├── ex2data1.txt                    # Student admission dataset
│   └── ex2data2.txt                    # Microchip quality dataset
├── utils.py                            # Helper functions for plotting, data loading
└── README.md                           # This file
```

---

## 🧰 Requirements

- Python 3.8+
- NumPy
- Matplotlib
- (Optional) Google Colab for running interactively

---

## 🚩 Usage

1️⃣ Clone the repository:
```bash
git clone https://github.com/your-username/logistic-regression-classification.git
cd logistic-regression-classification
```

2️⃣ Run the notebook:
- Open `logistic_regression_project.ipynb` in Jupyter or Colab.
- Run all cells to follow the structured learning workflow.

3️⃣ Analyze:
- Review **plots and outputs** to understand how logistic regression behaves on linear vs. non-linear problems.

---

## 🛡️ Learning Outcomes

✅ Understand and implement logistic regression from scratch.  
✅ Grasp the intuition and math behind sigmoid, cost, gradients, and optimization.  
✅ Appreciate the role of regularization in non-linear boundary problems.  
✅ Build confidence for **machine learning interviews, practical projects, and ML competitions**.

---

## ✍️ Author

**Mahmoud Mohamed Abas Mohamed**  
🗓️ May 18, 2025

---
