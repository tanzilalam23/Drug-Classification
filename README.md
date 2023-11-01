Drug Classification Analysis
Table of Contents
Overview
Dataset
Data Preprocessing
Univariate Analysis
Model Implementation
Results

Overview
This repository contains the code for drug classification analysis. The analysis includes data preprocessing, exploratory data analysis, and model implementation for classifying drugs based on several parameters.

Dataset
The dataset used for analysis is named drug.csv. It contains information on drug classification based on various attributes such as Age, Sex, Blood Pressure (BP), Cholesterol, Sodium to Potassium Ratio (Na_to_K), and the corresponding Drug category.

Data Preprocessing
The dataset was preprocessed to handle null values and encode categorical variables using Label Encoding techniques. The unique data features were explored, and the numerical data underwent univariate analysis to understand their distributions.

Univariate Analysis
Univariate analysis was performed on the numerical features 'Age' and 'Na_to_K'. The 'Na_to_K' feature exhibited right-skewed behavior and was transformed using a logarithmic scale for normalization.

The target variable 'Drug' showed an imbalance in labels, particularly an abundance of 'DrugY', influencing the implementation of class weights during model training to address this imbalance.

Model Implementation
The K-Nearest Neighbors (KNN) classification algorithm was implemented to classify drugs. The dataset was split into training and testing sets. Feature scaling using StandardScaler was applied before training the model.

The KNN model was trained using cross-validation techniques with varying 'n_neighbors' values. Confusion matrices and performance metrics were calculated for evaluating the model's accuracy, precision, and recall scores.

Results
The KNN model achieved an accuracy score of 80%. Analysis on different 'n_neighbors' values revealed the model's accuracy with varying numbers of neighbors.
