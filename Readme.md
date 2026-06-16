# Bangalore House Price Prediction

A machine learning project that predicts residential property prices in Bangalore based on key housing features such as location, area type, availability status, number of bedrooms, bathrooms, and total square footage. The project includes data cleaning, feature engineering, model comparison, training, and deployment through a Streamlit web application.

## Project Overview

The goal of this project is to build an accurate house price prediction model using real estate data from Bangalore. Various machine learning regression algorithms were evaluated, and the best-performing model was selected and deployed as an interactive web application.

## Features
- Comprehensive data cleaning and preprocessing
- Handling missing values and inconsistent data
- Custom square-footage conversion for different measurement units
- Outlier detection and removal
- Feature engineering
- Comparison of multiple regression models
- House price prediction through a Streamlit web interface
- Model serialization using Pickle

## Dataset
The project uses the Bangalore Housing Dataset containing features such as:

- Area Type
- Availability
- Location
- Number of Bedrooms (BHK)
- Number of Bathrooms
- Total Square Feet
- Price

## Data Preprocessing
The following preprocessing steps were performed:

- Removed rows with excessive missing values.
- Filled missing location values.
- Extracted BHK information from the size column.
- Converted different area measurements into square feet.
- Handled range-based square footage values.
- Removed unrealistic and extreme outliers.
- Created additional features:
- Price per square foot
- Square feet per BHK
- Removed highly skewed and inconsistent records.

## Exploratory Data Analysis
Several visualizations were created to understand the dataset:

- House price distribution
- Correlation heatmap
- Feature relationships
- Outlier analysis

## Models Evaluated
The following regression algorithms were compared:

- Linear Regression
- Lasso Regression
- Ridge Regression
- XGBoost Regressor
- Random Forest Regressor
- AdaBoost Regressor
- Gradient Boosting Regressor
- Decision Tree Regressor

Performance was evaluated using:

- R² Score
- Mean Squared Error (MSE)
- Model Pipeline

The final pipeline includes:

- One-Hot Encoding of categorical features:
- Area Type
- Availability
- Location
- Feature Scaling using StandardScaler
- XGBoost Regressor for prediction

The trained model was saved using Pickle for deployment.

Web Application

A Streamlit application was developed to provide real-time house price predictions.

User Inputs
Area Type
Availability Status
Location
Number of Bathrooms
Number of Bedrooms (BHK)
Total Square Footage

## Output
The application predicts the approximate market price of the property in Indian Rupees.

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-Learn
- XGBoost
- Matplotlib
- Seaborn
- Streamlit
- Pickle

## Future Improvements
Hyperparameter tuning using GridSearchCV
Improved location clustering
Model explainability using SHAP
Interactive analytics dashboard

## Results
The project successfully demonstrates the end-to-end machine learning workflow, from data preprocessing and feature engineering to model deployment. The deployed application allows users to estimate Bangalore house prices based on property characteristics quickly and efficiently.