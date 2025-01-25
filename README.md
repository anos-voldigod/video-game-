# video game market analysis

## Overview
This project aims to predict global sales of video games based on various features such as platform, genre, year of release, and publisher. The dataset contains information about video games, including their sales in different regions. By applying machine learning techniques, we train a regression model to predict the continuous target variable, Global_Sales.

## Project Workflow
1. Data Preprocessing
Missing Values: Rows with missing values are removed.
Categorical Encoding: Categorical features (Platform, Genre, Publisher) are encoded using pd.factorize().
Scaling: Continuous features are scaled using StandardScaler for normalization, ensuring all features contribute equally to the model.
2. Feature Engineering
Principal Component Analysis (PCA): Used to reduce feature dimensions while retaining 95% variance in the data.
Feature Selection: Used SelectKBest to choose the top features contributing to the target variable.
3. Modeling
Model Used: HistGradientBoostingRegressor, a fast and efficient regression algorithm, was chosen for its performance on large datasets and ability to handle missing values.
Hyperparameter Tuning: Used GridSearchCV to find the best combination of hyperparameters (learning rate, max depth, iterations).
4. Evaluation
Evaluation metrics include:
R² Score: Measure of how well the model explains variance.
RMSE (Root Mean Squared Error): Indicates average prediction error.
MAE (Mean Absolute Error): Measures the average magnitude of errors.
SHAP values are used for explainability to interpret feature importance.

## Results 
Accuracy : 0.80
