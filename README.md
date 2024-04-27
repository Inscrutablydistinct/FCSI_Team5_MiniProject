# FCSI_Team5_MiniProject

## Overview

This code offers a comprehensive analysis of NBA player salaries for the 2022-2023 season. By leveraging statistical methods, data visualization techniques, and machine learning models, it aims to uncover insights into the factors influencing player salaries in the NBA.

## Code Components

1. Loading and Exploring Data
The code loads NBA salary data from a CSV file and explores some features.
It provides an initial exploration of the dataset, including basic statistics and the identification of features with missing values.

2. Salary Distribution Analysis
Visualizes the distribution of player salaries using a histogram.
Categorizes salaries into ranges and presents the frequency distribution using a count plot.


<img src = "https://github.com/Inscrutablydistinct/FCSI_Team5_MiniProject/assets/121133033/33ef9a01-d88f-434d-810b-a3db45d8130b" width="400" height="300">
<img src = "https://github.com/Inscrutablydistinct/FCSI_Team5_MiniProject/assets/121133033/8657313e-a37a-4691-aad1-4fa846f62b06=150x150" width="400" height="300">
<img src = "https://github.com/Inscrutablydistinct/FCSI_Team5_MiniProject/assets/121133033/aa13a9cf-06b5-4b29-8f5a-669ce8a76fae=150x150" width="400" height="300">

3. Data Cleaning
Boxplot of top NBA Salary Predictors.
Anomaly Detection to detect outliers - PCA Visualization (Principal Component Analysis).
MP (Minutes Played) Bar Graph.
Feature engineering to create 3 new variables MP_Grade, TRB_Category, GS_Grade.
We also used data imputation as a part of feature engineering to substitute the missing values with the mean values of that particular column.
<img src = "https://github.com/Inscrutablydistinct/FCSI_Team5_MiniProject/assets/121133033/96632b30-37c5-4ace-8b23-f8b42be6e509" width="400" height="300">
<img src = "https://github.com/Inscrutablydistinct/FCSI_Team5_MiniProject/assets/121133033/0ed4b00e-e29f-4658-82a6-0ba7748ec319" width="400" height="300">

4. Correlation Analysis
Calculates the correlation between player salaries and other numerical features such as games played, total rebounds, and points scored.
Identifies features that exhibit high correlation with player salaries through a correlation matrix heatmap. Visualizes the correlation matrix heatmap.
<img src = "https://github.com/Inscrutablydistinct/FCSI_Team5_MiniProject/assets/121133033/96005f92-5e81-44f3-b6d6-e293e8c6f466" width="400" height="300">

5. Player Statistics Analysis
Explores the relationship between various player statistics (e.g., total rebounds, games started) and their impact on salaries.
Utilizes statistical tests (e.g., Shapiro-Wilk, Levene's) to assess the distribution and homogeneity of player statistics.
<img src = "https://github.com/Inscrutablydistinct/FCSI_Team5_MiniProject/assets/121133033/aaa88acc-132f-4957-a38c-380e26581fe0" width="400" height="300">
<img src = "https://github.com/Inscrutablydistinct/FCSI_Team5_MiniProject/assets/121133033/256a165b-3ea7-48b9-a007-1a0492c4496a" width="400" height="300">

6. Machine Learning Models
Implements machine learning models to predict player salaries based on their statistics.
Utilizes regression models including Linear Regression, Random Forest Regressor, Polynomial Regression, and XGBoost Regressor.
Employs cross-validation techniques to evaluate model performance and assess generalization to unseen data.
<img src = "https://github.com/Inscrutablydistinct/FCSI_Team5_MiniProject/assets/121133033/9ba6959e-9e32-4a08-967f-8cec750af849" width="400" height="300">
<img src = "https://github.com/Inscrutablydistinct/FCSI_Team5_MiniProject/assets/121133033/57b7a960-539a-4742-8831-e2a86413b10e" width="400" height="300">

7. Neural Network Modeling
Constructs a neural network using PyTorch to predict player salaries.
Defines the network architecture, loss function, and optimization algorithm.
Trains the model on the dataset and evaluates its performance using metrics such as Mean Squared Error and R^2 Score.
Usage

## Summary

Approaches used:-
•	Linear Regression
•	Random Forest
•	Polynomial Regression
•	XGBoost Regression

Generation of Machine Learning Model
To generate the Random Forest Model and Neural Network we used all the variables including the three categorical variables that we created – FG, FGA, 2P, 2PA, FT, FTA, PTS, MP_Grade, TRB_Category, GS_Grade.
To generate the other models we used only the numerical variables besides the three categorical variables presented to us – FG, FGA, 2P, 2PA, FT, FTA, PTS.

Explained Variances:-

Linear Regression:
-With Outliers - 0.59
-Without Outliers - 0.48

Random Forest (with cross-validation): 
With Categorical Variables & the other 7 variables - 0.45
The other 7 variables Without Categorical Variables - 0.60

Polynomial Regression - 0.66

Neural Network - -0.60

XGBoost Regression - 0.73

Dependencies

Pandas
Matplotlib
Seaborn
NumPy
Scikit-learn
XGBoost
PyTorch

Note
To run the code - 
Ensure that the required Python libraries (Pandas, Matplotlib, Seaborn, NumPy, Scikit-learn, XGBoost, PyTorch) are installed.
Place the NBA salary data CSV file in the appropriate directory.
Run the code in a Python environment such as Jupyter Notebook or a Python script.
