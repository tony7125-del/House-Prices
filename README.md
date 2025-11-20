House Price Prediction Project
Project Overview
This project focuses on predicting house prices using multiple linear regression and regularization techniques such as Ridge and LASSO regression. The goal is to build, interpret, and validate linear models that estimate house prices based on various property and neighborhood features. The project mimics a real-world workflow suitable for a data science portfolio.

Dataset
Filename: housepricesportfolio.csv

Number of observations: 500

Features include:

Property characteristics: LotSize, Bedrooms, Bathrooms, HouseAge, Renovated, GardenSize

Location and environment: DistancetoCityCenter, CrimeRate, NearbySchools, NoiseLevel

Socioeconomic indicators: MonthlyIncome, EnergyEfficiencyScore

Target variable: HousePrice (in 1,000s)

Problem Statement
A real-estate analytics team aims to estimate house prices in a city using the given features. The key tasks are to:

Explore the dataset and understand feature relationships.

Build a Multiple Linear Regression model and interpret results.

Validate model assumptions: linearity, independence, homoscedasticity, normality, multicollinearity, and outliers.

Apply variable selection and regularization using Ridge (L2) and LASSO (L1) to improve model generalization.

Save and load the best-performing model for future use.

What You'll Learn
Data loading and exploratory data analysis (EDA).

Construction and interpretation of a Multiple Linear Regression model.

Checking regression assumptions via plots and statistical tests.

Understanding overfitting and model generalization with train-test split evaluation.

Model improvement through Ridge and LASSO regularization techniques.

Model persistence using pickle.

Methodology
Data Preparation
Loaded data using pandas and performed initial EDA to understand feature distributions and correlations.

Split data into training and testing sets using an 80-20 ratio.

Modeling
Built baseline multiple linear regression using scikit-learn.

Examined coefficients and statistical significance with OLS regression (using statsmodels).

Evaluated model performance using Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R² score on training and testing sets.

Assumption Validation
Tested for linearity, normality, multicollinearity (using Variance Inflation Factor), homoscedasticity (using Breusch-Pagan test), and independence (using Durbin-Watson test).

Regularization
Applied Ridge (L2) and LASSO (L1) regression to reduce overfitting and improve model robustness.

Compared model performances and selected the best model.

Model Persistence
Saved the best model to disk using pickle for future predictions.

Demonstrated loading and using the persisted model.

Results
Achieved an approximate train R² of 0.69 and test R² of 0.53 indicating moderate predictive performance.

Coefficients aligned with domain expectations, e.g., positive impact of bedrooms and bathrooms on price, negative impact of distance to city center.

Regularization improved model generalization on unseen data.

Validated key assumptions as much as possible given the data.

Usage
To replicate or use the project:

Ensure all dependencies are installed (pandas, numpy, matplotlib, seaborn, scikit-learn, statsmodels, pickle).

Load the dataset housepricesportfolio.csv.

Run the notebook cells in sequence to execute EDA, modeling, validation, regularization, and model saving/loading.
