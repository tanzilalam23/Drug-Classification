# Drug Classification Analysis

## Overview

This project focuses on analyzing a drug classification dataset. The analysis includes data preprocessing, model implementation, and performance evaluation.

## Dataset

- **Source:** `drug.csv`
- **Description:** The dataset contains information about drug classifications based on attributes like Age, Sex, Blood Pressure (BP), Cholesterol, Sodium to Potassium Ratio (Na_to_K), and the corresponding drug label.

## Data Preprocessing

- Checked for missing values (None found).
- Encoded categorical variables using Label Encoding.
- Explored unique values for each categorical attribute.

## Univariate Analysis

- Conducted univariate analysis for numerical attributes: 'Age' and 'Na_to_K'.
- Applied log transformation to 'Na_to_K' to achieve a normal distribution.

## Model Implementation

- Utilized K-Nearest Neighbors (KNN) classifier for drug classification.
- Split the dataset into training and testing sets.
- Applied Standard Scaling for feature scaling.
- Explored different 'n_neighbors' values in KNN.
- Evaluated the model using confusion matrices and performance metrics.

## Results

- Achieved an accuracy of 80%.
- Investigated the impact of 'n_neighbors' on model performance.
