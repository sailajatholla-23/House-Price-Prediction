# House Price Prediction Using Machine Learning

## Project Overview

This project focuses on predicting residential house sale prices using machine learning regression techniques. The project uses the Ames Housing dataset, which contains information about various property characteristics that influence house prices.

The objective is to build and evaluate regression models, understand the relationship between property features and sale prices, and identify the best-performing model among those evaluated.

## Problem Statement

The goal is to develop a machine learning model that estimates a house's sale price based on its features. The project also examines how property characteristics influence prices and explores how predictions can support home buyers in comparing properties according to their requirements.

## Project Objectives

* Perform data analysis to understand the housing dataset.
* Identify important property features related to sale prices.
* Handle missing values and preprocess numerical and categorical variables.
* Train and evaluate multiple regression models.
* Compare model performance using appropriate evaluation metrics.
* Identify the best-performing model among the evaluated models.
* Discuss data challenges and the techniques used to address them.

## Dataset Information

**Dataset:** Ames Housing Dataset

* Total records: 1,460
* Total columns: 81
* Input features: 80
* Target variable: `SalePrice`

The dataset includes information about property size, quality, location, construction year, basement, garage, and other housing characteristics.

The target variable, `SalePrice`, represents the property's sale price.

## Technologies Used

* **Programming Language:** Python
* **Data Analysis:** Pandas, NumPy
* **Data Visualization:** Matplotlib
* **Machine Learning:** Scikit-learn
* **Development Environment:** Jupyter Notebook

## Project Workflow

1. Dataset loading and inspection
2. Exploratory data analysis
3. Target variable analysis
4. Missing-value analysis and data preprocessing
5. Separation of numerical and categorical features
6. Train-test split
7. Model training
8. Model evaluation and comparison
9. Best-model selection
10. Final conclusions

## Data Preprocessing

The following preprocessing techniques were used:

* Missing numerical values were handled using median imputation.
* Missing categorical values were handled using most-frequent-value imputation.
* Numerical features were scaled using `StandardScaler`.
* Categorical features were encoded using `OneHotEncoder` with unknown-category handling.
* A train-test split was used to evaluate model performance on unseen data.

## Machine Learning Models

The following regression models were evaluated:

* Linear Regression
* Random Forest Regressor
* Gradient Boosting Regressor

## Model Evaluation Metrics

Model performance was compared using:

* **Mean Absolute Error (MAE):** Measures the average absolute difference between actual and predicted prices.
* **Root Mean Squared Error (RMSE):** Measures prediction error while penalizing larger errors more strongly.
* **R-squared (R²):** Indicates how much of the variation in sale prices is explained by the model.

## Results and Model Comparison

The models were evaluated using a held-out test dataset.

| Model                       | R² Score |
| --------------------------- | -------: |
| Linear Regression           |   0.8867 |
| Random Forest Regressor     |   0.8941 |
| Gradient Boosting Regressor |   0.9045 |

Gradient Boosting achieved the highest R² score among the evaluated models.

**Best-performing model:** Gradient Boosting Regressor

* MAE: 16,576.29
* RMSE: 27,062.17
* R² Score: 0.9045

These results indicate that Gradient Boosting performed best among the three evaluated models on the selected test dataset.

## Challenges Faced

* **Missing values:** Missing data was handled using suitable imputation strategies for numerical and categorical features.
* **High-cardinality categorical features:** One-hot encoding was used to convert categorical variables into a format suitable for machine learning.
* **Different feature scales:** StandardScaler was applied to numerical features.
* **Model selection:** Multiple regression models were compared using consistent evaluation metrics to identify the best-performing model.

## Project Notebook

The complete analysis, preprocessing workflow, model training, evaluation, visualizations, and conclusions are available in the Jupyter Notebook included in this repository.

**Notebook:** `House Price Prediction.ipynb`

## Conclusion

This project demonstrates the use of machine learning regression techniques to predict residential house sale prices using property-related features.

Among the evaluated models, Gradient Boosting achieved the highest R² score of approximately 0.905, along with an MAE of approximately 16,576 and an RMSE of approximately 27,062. Therefore, it was selected as the best-performing model for this project.

The project highlights the importance of data preprocessing, model evaluation, and comparison when developing predictive solutions for housing data.

