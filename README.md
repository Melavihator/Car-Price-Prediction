# Car Price Prediction Project

## Overview
This project aims to develop a predictive model to estimate car prices based on various independent variables. The model provides valuable insights into the factors influencing car pricing, which can be leveraged by management to make informed decisions about car design, business strategy, and market entry. 

## Business Goal
The primary objective of this project is to model the price of cars using available features, enabling management to understand how prices vary with different attributes. This understanding will assist in manipulating car designs and strategies to achieve target pricing levels and navigate pricing dynamics in new markets.

## Dataset
The dataset used for this project contains various attributes of cars, including:

- **Engine Location**
- **Brand**
- **Fuel Type**
- **Cylinders**
- **Horsepower**
- **Dimensions (e.g., wheelbase, length, width)**
- **Price** (target variable)

### Data Preparation
- The dataset was preprocessed to handle missing values, encode categorical variables, and standardize numerical features as necessary. 

## Methodology

### 1. Data Exploration
Conducted exploratory data analysis (EDA) to identify relationships between features and the target variable (price). This included visualizations and summary statistics to understand data distribution and correlations.

### 2. Model Development
Several regression models were implemented to predict car prices, including:
- **Linear Regression**
- **Decision Tree Regressor**
- **Random Forest Regressor**
- **Gradient Boosting Regressor**
- **Support Vector Regressor**

### 3. Hyperparameter Tuning
Performed hyperparameter tuning using Grid Search to optimize model performance for Random Forest and Gradient Boosting models. This process involved testing various combinations of parameters and selecting the best performing models based on cross-validated mean squared error (MSE).

### 4. Model Evaluation
Evaluated model performance using the following metrics:
- **R² (Coefficient of Determination)**: Indicates the proportion of variance in the target variable that is predictable from the independent variables.
- **Mean Squared Error (MSE)**: Measures the average of the squares of the errors—how far predictions deviate from actual values.
- **Mean Absolute Error (MAE)**: Represents the average absolute difference between predicted and actual values.

## Results
### Model Performance Metrics
| Model                      | R²      | MSE          | MAE       |
|----------------------------|---------|--------------|-----------|
| Linear Regression          | 0.7885  | 16,695,279.26| 2,810.39  |
| Decision Tree Regressor    | 0.8564  | 11,335,290.67| 2,114.98  |
| Random Forest Regressor    | 0.9550  | 3,553,911.78 | 1,329.16  |
| Gradient Boosting Regressor | 0.9313  | 5,422,293.16 | 1,688.14  |
| Support Vector Regressor    | -0.0999 | 86,833,688.89| 5,696.31  |

### Best Parameters for Random Forest
- **Max Depth**: 20
- **Min Samples Split**: 2
- **Number of Estimators**: 200

### Insights
- **Engine Location** and **Brand** significantly impact pricing.
- Vehicles with higher horsepower and certain fuel types command higher prices.
- The Random Forest model outperformed others, explaining approximately 95.5% of the variance in car prices.

## Recommendations
- **Feature Optimization**: Focus on features that significantly impact pricing for future car designs.
- **Market Strategy**: Tailor marketing and pricing strategies based on insights gained from the model.
- **Continual Model Improvement**: Regularly update the model with new data and features to maintain accuracy and relevance.

