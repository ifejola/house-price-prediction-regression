# Multiple Linear Regression – House Price Prediction

## Project Overview

This project applies Multiple Linear Regression to predict median house values using several housing characteristics.

The objective is to understand relationships between multiple predictor variables and house prices while developing practical skills in regression modeling and performance evaluation.

## Dataset

**housing.csv**

The dataset contains housing information, including:

- Longitude and latitude
- Housing median age
- Total rooms and bedrooms
- Population
- Households
- Median income
- Median house value

**Target Variable:** median_house_value

## Tools & Libraries

Python | Pandas | Matplotlib | Seaborn | Scikit-learn

## Methodology

### 1. Data Exploration

- Loaded and inspected the housing dataset.
- Examined feature distributions and relationships.
- Investigated missing values and housing price patterns.

### 2. Data Preparation

- Selected eight numerical predictor variables.
- Excluded the categorical ocean_proximity column from the regression features.
- Explored the effect of removing observations with median house values of $500,000.
- Prepared the dataset for modeling.

### 3. Train-Test Split

Divided the data into:

- 80% training data
- 20% testing data

Used random_state = 42 for reproducibility.

### 4. Multiple Linear Regression

Trained a Linear Regression model using Scikit-learn.

Examined:

- Model intercept
- Regression coefficients
- Training predictions
- Testing predictions

### 5. Model Evaluation

Evaluated regression performance using:

**Mean Absolute Error (MAE):** Measures the average absolute difference between actual and predicted values.

**R² Score:** Measures the proportion of variation in house prices explained by the model.

Compared training and testing performance to assess generalization.

### 6. Data Visualization

Created scatter plots comparing actual and predicted house values.

Used a reference line to visualize how closely predictions aligned with actual observations.

## Key Takeaways

- Multiple Linear Regression uses several input features to predict a continuous target.
- Regression coefficients help explain the relationship between predictors and the target.
- MAE and R² provide different perspectives on model performance.
- Comparing actual and predicted values helps identify prediction errors.
- Data preparation and the treatment of extreme values can influence model results.

## Learning Outcomes

- Multiple Linear Regression
- Feature selection
- Data cleaning
- Model training and prediction
- Regression coefficients and intercepts
- MAE and R² evaluation
- Actual versus predicted visualizations

## Future Improvements

- Encode categorical variables such as ocean_proximity.
- Evaluate multicollinearity.
- Explore feature scaling where appropriate.
- Compare regression performance before and after removing capped house values.
- Explore Ridge and Lasso Regression.
