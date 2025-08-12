# Breast Cancer Classifier

## Problem Statement

The goal of this project is to develop and evaluate a machine learning model capable of classifying breast cancer tumors as either malignant (cancerous) or benign (non-cancerous) based on various diagnostic measurements.

## Dataset

This project uses the **Breast Cancer Wisconsin (Diagnostic) Dataset**, which is a standard benchmark dataset in machine learning.
- **Source:** [scikit-learn Breast Cancer Dataset](https://scikit-learn.org/stable/datasets/toy_dataset.html#breast-cancer-dataset)

## Methods

My approach to building the classifier followed these key steps:

1.  **Exploratory Data Analysis (EDA):** I loaded the dataset and performed an initial analysis, including:
    - Checking the dataset's shape and structure.
    - Visualizing the distribution of the target variable to understand class balance.
    - Analyzing correlations between features, such as the strong relationship between `mean radius` and `mean perimeter`.

2.  **Preprocessing:** I prepared the data for modeling by:
    - Splitting the dataset into training and testing sets (80/20 split).
    - Scaling the features using `StandardScaler` to ensure all features contribute equally to the models.

3.  **Baseline Models:** I trained two baseline classification models to establish a performance benchmark:
    - **Logistic Regression:** A linear model that's a good starting point for binary classification problems.
    - **K-Nearest Neighbors (KNN):** A simple, instance-based model that classifies new data points based on their proximity to known data points.

## Baseline Results

Here are the performance metrics for the baseline models on the test set:

### Logistic Regression
- **Accuracy:** 0.9737
- **Precision:** 0.9577
- **Recall:** 0.9937
- **F1-Score:** 0.9754

### K-Nearest Neighbors
- **Accuracy:** 0.9474
- **Precision:** 0.9598
- **Recall:** 0.9577
- **F1-Score:** 0.9598
