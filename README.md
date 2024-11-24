# Linear Regression Assignment

This project involves building and analyzing a multiple linear regression model to predict the demand for shared bikes. The notebook explores various statistical techniques, builds a predictive model, and evaluates its performance.

---

## **Project Objective**

BoomBikes, a bike-sharing service provider, aims to:
1. Understand the factors influencing bike demand.
2. Develop a predictive model to estimate future bike demand based on multiple variables.

The insights gained will help the company plan its strategies to meet demand efficiently and grow its business.

---

## **Dataset Overview**

The dataset includes daily observations of bike demand with features such as weather conditions, seasons, working days, and others. The dependent variable (`cnt`) represents the total count of bikes rented, and the independent variables represent potential factors affecting bike demand.

---

## **Key Steps**

### 1. **Exploratory Data Analysis (EDA)**
   - Analyzed and visualized the dataset for trends, patterns, and anomalies.
   - Identified relationships between features and target variable (`cnt`).

### 2. **Data Preprocessing**
   - Handled missing and duplicate data.
   - Transformed categorical variables (e.g., seasons, weather) into dummy variables.
   - Scaled numerical variables for consistent ranges.

### 3. **Feature Selection**
   - Evaluated the significance of variables using correlation analysis and Variance Inflation Factor (VIF) to avoid multicollinearity.
   - Applied Recursive Feature Elimination (RFE) for optimal feature selection.

### 4. **Model Building**
   - Built a linear regression model using the selected features.
   - Evaluated model performance using metrics such as R-squared, Adjusted R-squared, and F-statistic.

### 5. **Assumption Validation**
   - Validated linear regression assumptions:
     - Linearity
     - Normality of residuals (using Q-Q plot)
     - Homoscedasticity
     - Multicollinearity

### 6. **Model Interpretation**
   - Interpreted coefficients to understand the impact of variables on bike demand.
   - Identified significant predictors.

---

## **Results**

- **R-squared**: The proportion of variation in bike demand explained by the model.
- **Adjusted R-squared**: Adjusted for the number of predictors to avoid overfitting.
- Key findings:
  - Some features (e.g., `yr`, `workingday`, and `windspeed`) significantly influence bike demand.
  - Dummy variables for `season` and `weather` provide meaningful insights into demand variation.

---

## **Tools and Libraries**

- **Programming Language**: Python
- **Libraries**:
  - `pandas`, `numpy` - Data manipulation and analysis
  - `matplotlib`, `seaborn` - Visualization
  - `statsmodels`, `sklearn` - Statistical modeling and machine learning

---

## **Usage**

1. **Run the Notebook**: Open the `.ipynb` file in Jupyter Notebook or any compatible environment.
2. **Dataset**: Ensure the dataset file (`day.csv`) is in the same directory as the notebook.
3. **Requirements**: Install required Python libraries using `pip install -r requirements.txt`.

---

## **Future Enhancements**

1. Explore non-linear models or regularization techniques (Ridge, Lasso).
2. Address slight deviations in normality or outliers.
3. Incorporate external factors such as demographic data for better predictions.

---

## **Acknowledgment**

The dataset and problem statement were provided by BoomBikes as part of the consulting assignment to enhance their business operations.
