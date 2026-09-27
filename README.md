# -Linear-Regression---Project# 
# How Linear Regression Works & Learns
Linear regression is a method used to **predict a continuous value** based on one or more input features.  
It does this by finding the **best-fitting line (or hyperplane)** that minimizes the difference between the predicted values and the actual values.
---
## 1. Goal
Given:
- **Input features:** $X = [x_1, x_2, \dots, x_n]$
- **Target value:** $y$
We want to learn a model that predicts:
$$
\hat{y} = w_0 + w_1 x_1 + w_2 x_2 + \dots + w_n x_n
$$
Where:
- $w_0$ = **intercept** (bias term)
- $w_i$ = **weight** for feature $x_i$ (importance of the feature)
---
## 2. How the Model Learns
The learning process involves **finding the best weights ($w$)** so that predictions $\hat{y}$ are as close as possible to the actual values $y$.
**Step 1 – Initialize Weights**  
- Start with random values for $w_0, w_1, \dots, w_n$
**Step 2 – Make Predictions**  
- For each training example, calculate $\hat{y}$ using the current weights.
**Step 3 – Measure the Error**  
- Use the **Mean Squared Error (MSE)** loss function:
$$
\text{MSE} = \frac{1}{m} \sum_{i=1}^m (\hat{y}_i - y_i)^2
$$
Where $m$ is the number of training examples.

**Step 4 – Update Weights**  
- Apply **Gradient Descent** to reduce the error:
$$
w_j := w_j - \alpha \frac{\partial \text{MSE}}{\partial w_j}
$$
Where:
- $\alpha$ = learning rate (controls how big each update step is)
- $\frac{\partial \text{MSE}}{\partial w_j}$ = slope of the error curve w.r.t. $w_j$

**Step 5 – Repeat**  
- Keep adjusting the weights until:
  - The error stops decreasing significantly, or
  - A maximum number of iterations is reached.
---
## 3. Key Points
- **Strengths:** Simple, interpretable, and fast to train.
- **Limitations:** Assumes a linear relationship between features and target.
- **Extension:** Can be enhanced with polynomial features to capture non-linear patterns.
---
**Training Loop Summary:**  
1. Start with a rough line.  
2. Predict outputs for all data points.  
3. Compare predictions with actual values.  
4. Adjust weights to reduce error.  
5. Repeat until the best-fit line is found.
