# Sales-Forecast-Prediction


## Big Mart Sales Prediction

This project aims to predict the sales of products in Big Mart outlets using machine learning techniques, specifically sklearn and XGBoost.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Data Preprocessing](#data-preprocessing)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [Conclusion](#conclusion)
- [License](#license)

## Introduction
Predicting sales accurately is crucial for retail businesses to manage inventory, optimize operations, and increase revenue. This project leverages machine learning algorithms to predict the sales of various products at Big Mart outlets.

## Dataset
The dataset used is provided by [Kaggle](https://www.kaggle.com/competitions/big-mart-sales-data/). It contains information about various products and their sales across different stores.

## Project Structure
The project repository contains the following files:

- `BigMartSalesPrediction.ipynb`: Jupyter notebook with the complete analysis and model implementation.
- `README.md`: This readme file.

## Installation
To run this project locally, you need to have Python and Jupyter Notebook installed. You can install the required libraries using pip:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost
```

## Data Preprocessing
Data preprocessing steps include:

- Handling missing values in features like 'Item_Weight' and 'Outlet_Size'.
- Encoding categorical variables like 'Item_Type', 'Outlet_Location_Type', and 'Outlet_Type' using label encoding and one-hot encoding.
- Normalizing numerical features to standardize the scale.

## Feature Engineering
Feature engineering involves creating new features or modifying existing ones to improve model performance. In this project, the following steps were taken:

- Creating a new feature 'Outlet_Years' to represent the age of the store.
- Transforming 'Item_Fat_Content' to unify similar categories.
- Combining 'Item_Visibility' and 'Item_Type' to create an interaction feature.

## Modeling
The project uses two machine learning algorithms:

1. **Linear Regression (sklearn)**:
   - Splitting the data into training and testing sets.
   - Training the model using the training set.
   - Making predictions on the testing set.

2. **XGBoost**:
   - Utilizing XGBoost for better performance and handling complex relationships.
   - Hyperparameter tuning using GridSearchCV for optimal performance.

## Evaluation
The models' performances are evaluated using metrics like RMSE (Root Mean Squared Error) and R^2 Score. The following evaluation steps are included:

- Comparing the performance of Linear Regression and XGBoost.
- Plotting actual vs. predicted sales to visualize model accuracy.
- Analyzing feature importance from the XGBoost model.

## Conclusion
The XGBoost model generally outperforms Linear Regression in predicting Big Mart sales due to its ability to handle non-linear relationships and interactions between features. Further improvements could include additional feature engineering, more sophisticated hyperparameter tuning, and exploring other machine learning algorithms.

