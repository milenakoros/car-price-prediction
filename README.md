# DSC PJATK Recruitment: Car Price Prediction

This repository contains our solution for the DSC PJATK recruitment process. The goal of this project is to develop a predictive model that estimates car prices based on real data from online car advertisements.

## Task Description

The task requires building a regression model that predicts car prices using various features such as:
- **Brand and Model**
- **Year of Production**
- **Mileage**
- **Engine Power**
- **CO₂ Emissions**

The evaluation metric is RMSE (Root Mean Squared Error).

## Playbook Overview

Below is a step-by-step outline of what has been done in this notebook:

1. **Data Loading and Exploration**
   - **Import Libraries & Load Data:** All necessary Python libraries (e.g., pandas, matplotlib, scikit-learn) are imported and the dataset is loaded.
   - **Preliminary Analysis:** A brief analysis of the dataset is performed to understand data types, detect missing values, and review basic statistics.
   - **Exploratory Data Analysis (EDA):** Visualizations such as histograms, boxplots, and a correlation heatmap are used to uncover patterns and relationships between features.

2. **Data Cleaning and Preprocessing**
   - **Handling Missing Values:** Strategies to address missing data are applied (e.g., imputation or removal of rows with too many missing values).
   - **Outlier Detection:** Extreme values are identified and appropriately handled.
   - **Categorical Variables:** Text-based features (brand, model) are standardized and encoded.
   - **Feature Engineering:** New features (e.g., car age calculated from production year) are created to improve model performance.

3. **Model Building and Optimization**
   - **Data Splitting:** The data is divided into training and testing sets.
   - **Model Selection:** A `GradientBoostingRegressor` is chosen for regression.
   - **Hyperparameter Tuning:** `GridSearchCV` is used to tune parameters such as `n_estimators`, `learning_rate`, and `max_depth` with 3-fold cross-validation.
   - **Model Evaluation:** The model’s performance is assessed using metrics like MAE and RMSE.

4. **Final Model and Prediction**
   - **Best Model Selection:** The best estimator from the grid search is selected.
   - **Final Predictions:** The final model is used to make predictions on the test set, and the performance is evaluated.
   - **Optional Submission:** Predictions can be saved (e.g., in a CSV format) for further evaluation or submission if required.

5. **Conclusions**
   - **Insights:** Key findings from the EDA and feature importance are discussed.
   - **Future Improvements:** Suggestions for potential enhancements in model tuning and data preprocessing are provided.
