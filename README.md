# Public_Data_Prediction_Modeling
the goal is to predict where will be the optimized opening place for the new business. The data will be trained by merging public data and Yelp API. I will create a new equation to estimate the success rate based on review counts and counts of surrounding human waste.   

# Case Count Prediction Model

This repository contains code for building and evaluating machine learning models to predict case counts based on neighborhood information and geographical coordinates.

## Dataset

The dataset consists of two CSV files:
- `train_data.csv`: Training data containing features (Year, Neighborhood, Latitude, Longitude) and the target variable (Case_Count).
- `test_data.csv`: Test data containing features (Year, Neighborhood, Latitude, Longitude) for which case counts need to be predicted.

## Models

### Linear Regression

- Implemented using scikit-learn's `LinearRegression`.
- Assumes a linear relationship between input features and the target variable.
- Provides a baseline model for comparison and easy interpretability.

### Random Forest Regression

- Implemented using scikit-learn's `RandomForestRegressor`.
- Ensemble learning technique based on decision trees.
- Captures nonlinear relationships and handles high-dimensional data well.
- Robust to overfitting and generally provides accurate predictions.

### Lasso Regression

- Implemented using scikit-learn's `Lasso`.
- Performs both variable selection and regularization by adding a penalty term to the loss function.
- Useful for feature selection and dealing with high-dimensional data.

## Workflow

1. Data Preparation: Load the training and test data, preprocess features, and split the training data into train and validation sets.
2. Model Training: Train Linear Regression, Random Forest Regression, and Lasso Regression models using the training data.
3. Model Evaluation (Optional): Evaluate the models on the validation set using Mean Absolute Error (MAE).
4. Prediction: Predict case counts for the test data using the trained models.
5. Result Analysis: Compare and analyze the predictions from each model.


## Conclusion

Evaluate the performance of each model based on metrics like MAE and choose the best model for predicting case counts in your scenario.
