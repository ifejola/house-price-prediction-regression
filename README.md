# house-price-prediction-regression
Predicting housing prices using multiple linear regression with model evaluation (MAE, R²) and feature analysis
# House Price Prediction Using Linear Regression

## Overview
This project builds a multiple linear regression model to predict housing prices based on various features such as location, income, and housing characteristics.

The goal is to understand how different factors influence house prices and evaluate the model’s predictive performance.

---

## Dataset
The dataset contains 20,000+ housing records with features including:

- Longitude & Latitude
- Housing Median Age
- Total Rooms & Bedrooms
- Population & Households
- Median Income
- Median House Value (target variable)
- Ocean Proximity (categorical)

---

## Tools & Libraries
- Python
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

---

## Data Preparation

- Checked for missing values
- Removed null values using `dropna()`
- Dropped categorical column (`ocean_proximity`) since it requires encoding
- Selected only numerical features for modeling

---

## Feature Selection

**Predictors (X):**
- longitude
- latitude
- housing_median_age
- total_rooms
- total_bedrooms
- population
- households
- median_income

**Target (y):**
- median_house_value

---

## Model Building

- Split data into training (80%) and testing (20%)
- Used `LinearRegression` from scikit-learn
- Trained model on training dataset

---

## Model Interpretation

- Extracted coefficients to understand feature impact
- Identified how each variable influences house price
- Calculated intercept and feature weights

---

## Evaluation Metrics

- **Mean Absolute Error (MAE):** ~51,372  
- **R-squared (R²):** 0.64  

### Interpretation:
- The model explains ~64% of the variance in housing prices
- Indicates moderate predictive performance with room for improvement

---

## Results

- Generated predictions for housing prices
- Compared actual vs predicted values
- Observed differences to evaluate model accuracy

---

## Key Insights

- Median income has a strong positive impact on house prices  
- Location (latitude/longitude) significantly influences value  
- Some features contribute less and may be refined  

---

## Future Improvements

- Apply feature scaling (StandardScaler)
- Encode categorical variables (ocean_proximity)
- Try advanced models (Random Forest, Gradient Boosting)
- Perform feature engineering

---

## Conclusion

Linear regression provides a solid baseline model for predicting housing prices and understanding feature relationships, but more advanced techniques could improve performance.
