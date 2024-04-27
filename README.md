# FCSI_Team5_MiniProject


README
Table of Contents: -
1.	Problem Definition and Goal
2.	Exploratory Data Analysis
3.	Machine Learning and Problem Solving
4.	Data driven Insights.
Introduction-
The NBA is one of the most popular sports leagues and arguably the most popular basketball league in the world comprising of some of the most renowned and revered basketball players. Over time NBA player salaries have been rising continuously and right now the NBA is the highest paying sports league in the world with players earning 8.5million US dollars on average. Behind how salaries of nba players are determined lies a complex and diverse set of reasons and factors such points, FG, FGA etc.
Goal and Problem Definition: -
Goal - Determining the factors affecting the salary of an NBA player.
Problem Definition - What are the main factors that determine the salaries of NBA players?
Dataset description:
•	Name: nba_salary.csv
•	Collection of data of nba players who played in the 2022-2023 regular season
Exploratory Data Analysis:-
How we did it?
1.	Data Visualization
2.	Database Cleaning
3.	Data preparation
Models and Techniques Used:-
1.	Models - Salary range (Bar Graph)
2.	Heatmap
3.	Boxplot of top NBA Salary Predictors
4.	Anomaly Detection - PCA Visualization (Principal Component Analysis)
5.	MP (Minutes Played) Bar Graph 
6.	Feature engineering to create 3 new variables MP_Grade, TRB_Category, GS_Grade
7.	We also used data imputation as a part of feature engineering to substitute the missing values with the mean values of that particular column.
Machine Learning and Problem Solving
Approaches used:-
•	Linear Regression
•	Random Forest
•	Polynomial Regression
•	XGBoost Regression
Generation of Machine Learning Model
To generate the Random Forest Model we used all the variables including the three categorical variables that we created – FG, FGA, 2P, 2PA, FT, FTA, PTS, MP_Grade, TRB_Category, GS_Grade.
To generate the other models we used only the other variables besides the three categorical variable presented to us – FG, FGA, 2P, 2PA, FT, FTA, PTS.
Explained Variance:-
Linear Regression: 
-With Outliers - 0.59
-Without Outliers - 0.48
Random Forest (with cross validation): 
With Categorical Variables & the other 7 variables - 0.45
The other 7 variables Without Categorical Variables - 0.60
Polynomial Regression - 0.66
Neural Network - -0.60
XGBoost Regression - 0.73



NBA Salary Analysis ReadMe

Overview

This code provides an analysis of NBA player salaries for the 2022-2023 season. It includes visualizations, statistical insights, and machine learning models to understand the factors influencing player salaries.

Code Components

1. Loading and Exploring Data
The code loads NBA salary data from a CSV file and explores basic statistics.
It identifies features with missing values and prints the percentage of missing values for each feature.
2. Salary Distribution Analysis
Visualizes the distribution of salaries and categorizes them into ranges.
3. Correlation Analysis
Calculates the correlation between salary and other numerical features.
Identifies features highly correlated with salary.
Visualizes the correlation matrix heatmap.
4. Player Statistics Analysis
Analyzes the relationship between player statistics (e.g., total rebounds, games started) and salaries.
Applies machine learning models to predict salaries based on player statistics.
5. Statistical Tests and Categorization
Conducts statistical tests (Shapiro-Wilk and Levene's tests) on salary data.
Categorizes player statistics into bins for analysis.
6. Machine Learning Models
Utilizes various machine learning models to predict player salaries:
Linear Regression
Random Forest Regressor
Polynomial Regression
XGBoost Regressor
Neural Network
Usage

Ensure the necessary libraries (Pandas, Matplotlib, Seaborn, NumPy, Scikit-learn, XGBoost, PyTorch) are installed.
Place the NBA salary data CSV file in the appropriate directory.
Run the code in a Python environment (Jupyter Notebook or script).
Dependencies

Pandas
Matplotlib
Seaborn
NumPy
Scikit-learn
XGBoost
PyTorch
Note

This code assumes the availability of the NBA salary dataset for the 2022-2023 season in CSV format.
Adjustments may be required for different datasets or analysis goals.


