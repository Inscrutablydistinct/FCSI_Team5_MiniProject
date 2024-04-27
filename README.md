# FCSI_Team5_MiniProject

Overview

This code offers a comprehensive analysis of NBA player salaries for the 2022-2023 season. By leveraging statistical methods, data visualization techniques, and machine learning models, it aims to uncover insights into the factors influencing player salaries in the NBA.

Code Components

1. Loading and Exploring Data
The code begins by loading the NBA salary data from a CSV file using the Pandas library.
It provides an initial exploration of the dataset, including basic statistics and the identification of features with missing values.
2. Salary Distribution Analysis
Visualizes the distribution of player salaries using a histogram.
Categorizes salaries into ranges and presents the frequency distribution using a count plot.
3. Correlation Analysis
Calculates the correlation between player salaries and other numerical features such as games played, total rebounds, and points scored.
Identifies features that exhibit high correlation with player salaries through a correlation matrix heatmap.
4. Player Statistics Analysis
Explores the relationship between various player statistics (e.g., total rebounds, games started) and their impact on salaries.
Utilizes statistical tests (e.g., Shapiro-Wilk, Levene's) to assess the distribution and homogeneity of player statistics.
5. Machine Learning Models
Implements machine learning models to predict player salaries based on their statistics.
Utilizes regression models including Linear Regression, Random Forest Regressor, Polynomial Regression, and XGBoost Regressor.
Employs cross-validation techniques to evaluate model performance and assess generalization to unseen data.
6. Neural Network Modeling
Constructs a neural network using PyTorch to predict player salaries.
Defines the network architecture, loss function, and optimization algorithm.
Trains the model on the dataset and evaluates its performance using metrics such as Mean Squared Error and R^2 Score.
Usage

Ensure that the required Python libraries (Pandas, Matplotlib, Seaborn, NumPy, Scikit-learn, XGBoost, PyTorch) are installed.
Place the NBA salary data CSV file in the appropriate directory.
Run the code in a Python environment such as Jupyter Notebook or a Python script.
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
Adjustments may be necessary for different datasets or analysis goals.

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





