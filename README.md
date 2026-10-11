# Linear and Logistic Regression Projects 

An educational repository dedicated to implementing fundamental machine learning algorithms: **Linear Regression** and **Logistic Regression** as part of practical lab works (TPs).

---

##  Repository Structure

The project is organized into dedicated directories to maintain a clean workspace:

*   📂 **[TP1_Linear_Regression](./TP1_Linear_Regression):** Contains files related to the first practical assignment on Linear Regression:
    *   `Simple_Linear_regression_model.ipynb` — Implementation of a simple linear regression model.
    *   `TP1_Linear_Regression_Load_the_Dataset_from_GitHub.ipynb` — Guide on fetching the dataset directly from GitHub.
    *   `StudentPerformanceFactors.csv` — The dataset used for predicting student performance factors.
*   📂 **[TP2_Logistic_Regression](./TP2_Logistic_Regression):** Contains files and models related to the second practical assignment on Logistic Regression for classification tasks.

---

##  Theoretical Overview

### 1. Linear Regression
Used to predict a continuous target value based on given input features. The goal is to fit a line (or hyperplane) that minimizes the difference between predicted and actual values using the **Mean Squared Error (MSE)** loss function and **Gradient Descent** optimization.

\[\hat{y} = w_0 + w_1 x_1 + w_2 x_2 + \dots + w_n x_n\]

### 2. Logistic Regression
Used for binary classification problems (e.g., pass/fail). It maps the linear model outputs to a probability value between 0 and 1 by passing it through the **Sigmoid Function**.

\[P(y=1\vert{}x) = \sigma(w^T x) = \frac{1}{1 + e^{-w^T x}}\]

