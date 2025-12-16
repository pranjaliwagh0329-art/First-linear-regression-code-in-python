# First-linear-regression-code-in-python
 Project Overview: Linear Regression Model
This code file demonstrates how to build and interpret a Linear Regression model using Python. The goal is to understand how multiple input features affect a target variable and to extract the learned model parameters.

🔧 Libraries Used
NumPy – for numerical operations
Pandas – for data handling
scikit-learn – to build and train the Linear Regression model

🧠 Model Creation

A Linear Regression model is created using LinearRegression() from sklearn.linear_model.
The model learns a linear relationship between the input features (X) and the target variable (y).

🏋️ Model Training

The model is trained using:
linreg.fit(X, y)
This step allows the algorithm to learn:
How much each feature influences the target
The best-fit line that minimizes prediction error

📊 Model Parameters
1️⃣ Intercept
print(linreg.intercept_)
Output:
-11.278686999420255
🔹 This is the intercept (bias) of the model.
It represents the predicted value of the target when all input features are zero.

2️⃣ Coefficients
linreg.coef_
Output:
[ 0.15983489,  0.26387788, -0.62395481,  0.37014516, -0.25123053 ]


🔹 These are the coefficients (weights) for each feature.
Positive values → feature increases the target value
Negative values → feature decreases the target value
Higher magnitude → stronger impact on prediction
Each coefficient corresponds to one input feature in X.

📐 Mathematical Representation

The trained model follows this equation:
y = (0.1598 × X1) + (0.2639 × X2) − (0.6240 × X3)
    + (0.3701 × X4) − (0.2512 × X5) − 11.2787

✅ Conclusion

This code successfully builds a multiple linear regression model
It extracts and interprets:
Intercept
Feature coefficients

Useful for prediction, feature impact analysis, and machine learning basics
