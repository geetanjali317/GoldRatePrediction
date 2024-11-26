# GoldRatePrediction
This project aims to predict gold prices using various linear regression models. The dataset used is FINAL_USO.csv, which contains historical data related to gold prices. The models implemented are Linear Regression, Lasso Regression, Ridge Regression, and ElasticNet Regression.
Table of Contents

    Overview
    Dataset
    Modeling Techniques
    Evaluation Metrics
    Results
    Installation
    Usage
    License

Overview

This project uses multiple linear regression models to predict gold prices. The goal is to determine which model provides the most accurate predictions based on the provided dataset. The models used in this project include:

    Linear Regression
    Lasso Regression
    Ridge Regression
    ElasticNet Regression

Dataset

The dataset FINAL_USO.csv contains historical data for predicting gold prices. The features in the dataset are related to gold price fluctuations, and the target variable is the gold price.
Example of columns in the dataset:

    Date: Date of the data point
    Gold_Price: Price of gold (target variable)
    Other relevant features related to gold price prediction

Modeling Techniques
1. Linear Regression

Linear regression is a basic approach to modeling the relationship between the dependent variable (gold price) and independent variables. It assumes a linear relationship.
2. Lasso Regression

Lasso (Least Absolute Shrinkage and Selection Operator) regression is a regularized version of linear regression that performs both variable selection and regularization, which can help prevent overfitting.
3. Ridge Regression

Ridge regression is another regularized linear regression method, which penalizes large coefficients and helps to prevent overfitting. It is particularly useful when the dataset has multicollinearity.
4. ElasticNet Regression

ElasticNet is a regularized regression method that combines Lasso and Ridge regression penalties, balancing both L1 and L2 regularization. It is useful when there are correlations between features.
Evaluation Metrics

The following metrics are used to evaluate the models:

    Mean Absolute Error (MAE): Measures the average magnitude of the errors in a set of predictions, without considering their direction.
    Mean Squared Error (MSE): Measures the average of the squares of the errors—that is, the average squared difference between the estimated values and the actual value.
    R² (R-Squared): A statistical measure that represents the proportion of the variance for a dependent variable that's explained by the independent variables in the model.

Results
1. Linear Regression

    MAE: 9.62e-14
    MSE: 1.22e-26
    R²: 1.0 (Perfect fit)

2. Lasso Regression

    R²: 0.9966
    MSE: 0.9999
    MAE: 0.7427

3. Ridge Regression

    R²: 0.9999
    MSE: 0.0425
    MAE: 0.1317

4. ElasticNet Regression

    R²: 0.9824
    MSE: 5.24
    MAE: 1.8847

Installation

To run this project, you need to install the required dependencies. You can do this using pip:

pip install -r requirements.txt

The requirements.txt file should include the following libraries:

    pandas
    numpy
    matplotlib
    seaborn
    scikit-learn

Usage

Once you have installed the necessary libraries and dependencies, you can run the Python scripts in this project to train and evaluate the regression models.

    Load the dataset: Ensure that FINAL_USO.csv is in the project directory or specify its path.

    Train the models: The script will automatically train the Linear Regression, Lasso, Ridge, and ElasticNet models using the dataset.

    Evaluate the models: After training, the script will output the evaluation metrics (MAE, MSE, R²) for each model.

    Make predictions: Once the models are trained, you can use them to predict gold prices using the predict() function.

License

This project is licensed under the MIT License - see the LICENSE file for details.
