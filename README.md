# Credit-Score-Classification

This repository contains a project for classifying credit scores into three categories: Good, Standard, and Bad. The project involves performing Exploratory Data Analysis (EDA) and building machine learning models.

## Project Overview
The goal of this project is to predict the credit score of customers using various features in the dataset. The project is divided into two main parts:

Exploratory Data Analysis (EDA)   
Machine Learning Model Building

## Dataset

The dataset used in this project contains 100000 records, each representing an individual's financial and credit history. It includes various features that provide insights into an individual's credit behavior and financial status, enabling the classification of their credit score.   
The target variable is the credit score, classified into three categories:

* Good
* Standard
* Poor

You can download the dataset from Kaggle using this [link](https://www.kaggle.com/datasets/parisrohan/credit-score-classification/data).

## Project Workflow
1. Data Preprocessing:
   - Handle missing values.
   - Encode categorical variables.
   - Split the dataset into training and testing sets.
  
2. Model Training:
   - Train multiple machine learning models.
   - Use cross-validation for model evaluation.
  
3. Model Evaluation:
   - Evaluate models based on F1 score.
   - Select the best-performing model.

4. Feature Importance:
   - Analyze the importance of features in the best-performing model.

5. Conclusion:
   - Summarize findings and potential improvements.

## Exploratory Data Analysis (EDA)
The EDA was conducted to understand the structure of the data, handle missing values, and visualize the distribution of variables. Key steps included:

* Checking for missing values and data types
* Cleaning and preprocessing data to handle noise/inappropriate entries
* Visualizing the distribution of the target variable
* Plotting correlations between features

## Machine Learning
The machine learning file (ML.ipynb) includes the following steps:
* Importing necessary libraries
* Loading the cleaned dataset
* Splitting the data into training and testing sets
* Building classification models (KNN, Decision Tree, Random Forest, AdaBoost with Random Forest, Gradient Boosting,  XGBoost)
* Hyperparameter tuning using GridSearchCV
* Evaluating the models using F1 Score, confusion matrix, and classification report
  Making predictions on the test data

## Results
The performance of the models was evaluated using cross-validation with the F1 score as the primary metric. Among all models, the Boosted Random Forest achieved the highest performance.

## Model Performance

|Model |	Mean F1 Score |	Std F1 Score
|----- | -------------- | ------------ |
|KNN |	0.681 |	0.011 |
|Decision Tree |	0.649 |	0.005 |
|Random Forest |	0.718 |	0.008 |
|Boosted RF |	0.745 |	0.007 |
|Gradient Boosting |	0.715 |	0.006 |

## Conclusion
The Boosted Random Forest model achieved the highest performance with an F1 score of 74.4%, indicating a good balance between precision and recall. This makes it the most effective model for this credit score classification problem.
