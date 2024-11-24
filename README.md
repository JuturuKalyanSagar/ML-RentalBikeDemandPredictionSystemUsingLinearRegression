# Rental bike demand prediction system

## Overview
This project involves building and analyzing a multiple linear regression model to predict the demand for shared bikes in different seasons, days etc. This project explores various statistical techniques, builds a predictive model, and evaluates its performance.

---

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information

BoomBikes, a bike-sharing service provider, wants to:
1. Understand the factors influencing bike demand.
2. Develop a predictive model to estimate future bike demand based on multiple variables.

The insights gained from this will help the company plan its strategies to meet demand efficiently and grow its business further.

---

## **Dataset Overview**

The dataset includes daily observations of bike demand with features such as weather conditions, seasons, working days, and others. The dependent variable (`cnt`) represents the total count of bikes rented, and the independent variables represent potential factors affecting bike demand.

---

## **Key Steps**

### 1. **Exploratory Data Analysis (EDA)**
   - Analyzed and visualized the dataset for trends, patterns, and anomalies.
   - Identified relationships between features and target variable (`cnt`).

### 2. **Data Preprocessing**
   - Transformed categorical variables (e.g., seasons, weather) into dummy variables.
   - Scaled numerical variables for consistent ranges using Min-Max scaler.

### 3. **Feature Selection**
   - Evaluated the significance of variables using correlation analysis and Variance Inflation Factor (VIF) to avoid multicollinearity.
   - Applied Recursive Feature Elimination (RFE) for optimal feature selection.

### 4. **Model Building**
   - Built a linear regression model using the selected features.
   - Evaluated model performance using metrics such as R-squared, Adjusted R-squared etc.

### 5. **Assumption Validation**
   - Validated linear regression assumptions:
     - Linearity
     - Normality of residuals (using Q-Q plot)
     - Multicollinearity

### 6. **Model Interpretation**
   - Interpreted coefficients to understand the impact of variables on bike demand.
   - Identified final significant predictors.

---

## **Results**

- **R-squared**: The proportion of variation in bike demand explained by the model.
- **Adjusted R-squared**: Adjusted for the number of predictors to avoid overfitting.
- Key findings:
  - Some features (e.g., `yr`, `workingday`, and `windspeed`) significantly influence bike demand.
  - Dummy variables for `season` and `weather` provide meaningful insights into demand variation.
  
---
  
## Conclusions
This case study provided analysis of Rental bike demand. Using this BoomBikes can predict rental bikes demand and shall plan to improve their business based on these factors.

---

## Technologies Used

The project was built using the following technologies:
- **Python**: For data manipulation, analysis, and modeling.
- **Pandas & NumPy**: For data manipulation and numerical operations.
- **Matplotlib & Seaborn**: For data visualization.
- **statsmodels & sklearn**: Statistical modeling and machine learning.
- **Jupyter Notebook**: For interactive code development and documentation.

---

## Acknowledgements

- This project was inspired by Upgrad.
- This project was based on [Upgrad Learning](https://www.upgrad.com).

---

## Contact
Created by [@JuturuKalyanSagar] - feel free to contact me!
