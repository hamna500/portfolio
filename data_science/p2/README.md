# E-commerce Dataset Analysis Part 2

## Overview

Welcome to the E-commerce Dataset Analysis Part 2 project! This analysis aims to train linear regression models for predicting users' ratings towards items using an e-commerce dataset. By following a comprehensive data science workflow, including data exploration, model training, prediction, and evaluation, we seek to gain insights into the impact of feature selection and training/testing data size on model performance.

## Dataset Import

### Description
The project utilizes a cleaned e-commerce dataset provided in the CSV format. This dataset contains information about user ratings, reviews, helpfulness, gender, category, and more.

### Import Process
The dataset is imported using the Pandas library's `read_csv` method. After importing, we explore the dataset's basic structure and information to gain initial insights.

## Dataset Exploration

### Overview
To understand the dataset better, we employ exploratory data analysis techniques, including:
- Displaying the first few rows of the dataset using the `head()` method.
- Obtaining a summary of the dataset's structure and data types using the `info()` method.

### Correlation Analysis
We calculate correlations between different features (such as helpfulness, gender, category, review) and ratings. This helps us identify which features are most correlated with ratings and understand potential relationships.

## Split Training and Testing Data

### Description
In machine learning, it's essential to split the dataset into training and testing sets to train the model and evaluate its performance, respectively.

### Process
We randomly split the dataset into training and testing sets using the `train_test_split` method from scikit-learn. Two scenarios are considered:
1. Case 1: Training data contains 10% of the entire dataset.
2. Case 2: Training data contains 90% of the entire dataset.

## Train Linear Regression Models with Feature Selection

### Description
Feature selection plays a crucial role in model training. We select the most correlated and least correlated features from the dataset to train four linear regression models.

### Process
- We train four linear regression models:
    - Model A: Most correlated features (Case 1)
    - Model B: Least correlated features (Case 1)
    - Model C: Most correlated features (Case 2)
    - Model D: Least correlated features (Case 2)
- The models are trained using the selected features and evaluated for their performance.

## Evaluate Models

### Description
Model evaluation is crucial to assess the effectiveness of trained models in making predictions.

### Metrics
We evaluate the models using two metrics:


## Mean Squared Error (MSE)
Mean Squared Error (MSE) is a common metric used to evaluate the performance of regression models. It measures the average squared difference between the predicted values and the actual values in the dataset. MSE is calculated as the sum of squared errors divided by the number of observations. A lower MSE indicates better model performance, with a value of 0 indicating perfect predictions.

The formula for MSE is:
MSE = (1/n) * Σ(yᵢ - ȳ)²


n is the number of observations.


yi is the actual value of the target variable for the 𝑖𝑡ℎ observation.

​
 ȳ is the predicted value of the target variable for the 𝑖𝑡ℎ observation.
 

## Root Mean Squared Error (RMSE)
Root Mean Squared Error (RMSE) is the square root of the MSE and is used to quantify the average magnitude of the errors in the predicted values. It is expressed in the same units as the target variable, making it easier to interpret. RMSE penalizes larger errors more heavily than smaller errors due to the squaring operation in MSE.

The formula for RMSE is:
RMSE = √MSE


Like MSE, a lower RMSE indicates better model performance, with a value of 0 indicating perfect predictions.

## Data Science Ethics

### Overview
Ethical considerations are essential in data science to ensure fairness, transparency, and accountability.

### Analysis
We conduct an ethical analysis of an infographic depicting the 2008 Summer Olympics medal tallies. Potential concerns related to bias, nationalistic sentiments, and underrepresentation of achievements are discussed. Emphasis is placed on promoting diversity and fairness in data presentation.

---

This detailed README provides a comprehensive overview of the project, including its objectives, dataset exploration, model training, evaluation, and ethical considerations. 
