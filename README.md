# Crab Age Prediction

## Overview
This project focuses on predicting the age of crabs based on various physical measurements such as weight, length, diameter, and shell weight. The goal is to develop a machine learning model that can accurately estimate the age of crabs, which is crucial for understanding crab growth and managing crab populations. This notebook was part of a university kaggle competition which scored first place with an MAE of 1.30587.

---

## Dataset
The dataset used in this project contains features about crabs such as weight, diameter, height, length and target variable Age. Link to the dataset is [here](https://drive.google.com/file/d/1Oqy19sw3kPHZ-T0G_-2xUDErNkLS6QTL/view?usp=sharing)

---

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/sarahelfeel04/Crab-Age-Prediction.git
   ```

2. Run the notebook and change file path of datasets

---

## Summary
1. **Exploratory Data Analysis (EDA)**:
   - **Data Loading**: Loaded the dataset and performed initial inspections to understand its structure.
   - **Data Cleaning**: Handled missing values, checked for duplicates, and ensured data consistency.
   - **Data Visualization**: Created visualizations to understand the distribution of features and their relationships. Used histograms, box plots, and scatter plots.
   - **Feature Engineering**: Generated new features that could potentially improve model performance, such as ratios and combined metrics.

2. **Data Preprocessing**:
   - **Normalization/Scaling**: Applied normalization and scaling techniques to prepare the data for machine learning models.
   - **Encoding Categorical Variables**: Encoded categorical variables (e.g., Sex) using one-hot encoding.
   - **Train-Test Split**: Split the dataset into training and testing sets to evaluate model performance.

3. **Model Training**:
   - **Model Selection**: Evaluated multiple machine learning models, including Linear Regression, Polynomial Regression, Quantile, RANSAC, Theil-Sen, Huber Regressors and LightGBM.
   - **Regularization**: Applied regularization techniques such as L1, L2 and Elastic Net to avoid overfitting.
   - **Hyperparameter Tuning**: Used grid search and cross-validation to find the best hyperparameters for each model.
   - **Model Evaluation**: Assessed model performance using Mean Absolute Error (MAE).

4. **Model Evaluation**:
   - **Performance Metrics**: Compared the performance of different models using MAE.
   - **Feature Importance**: Analyzed the importance of features in the best-performing model to understand their impact on predictions.
   - **Best Model**: LightGBM Regressor
