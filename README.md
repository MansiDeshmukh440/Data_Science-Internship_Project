## Summary of Exploratory Data Analysis (EDA) and Linear Regression on the Air Quality Dataset


1. Introduction
The Air Quality dataset contains measurements of various air pollutants in an unspecified European city. The goal of this analysis is to understand the relationships between different air pollutants and predict the concentration of carbon monoxide (CO) based on other sensor readings.


2. Data Overview
The dataset includes several columns, with key features being:


CO(GT): Concentration of CO in mg/m^3.
PT08.S1(CO): Tin oxide sensor from Gas1 (CO).
PT08.S2(NMHC): Non-metanic hydrocarbons.
PT08.S3(NOx): Tungsten oxide sensor from Gas2 (NOx).
PT08.S4(NO2): Tungsten oxide sensor from Gas3 (NO2).
PT08.S5(O3): Indium oxide sensor from Gas4 (O3).


3. Data Cleaning
Columns with all missing values were dropped.
Numerical columns had comma decimal separators replaced with periods to ensure correct float conversion.
Rows with any missing values were removed to avoid complications in the analysis.


4. Exploratory Data Analysis (EDA)
Descriptive Statistics: Provided insights into the central tendency, dispersion, and shape of the dataset's distribution.
Correlation Analysis: Examined the correlation between CO(GT) and other sensor readings. A heatmap visualized the correlation matrix to identify highly correlated variables.
Distribution Plots: Visualized the distribution of CO(GT) and other key features to understand their spread and skewness.


5. Linear Regression Analysis
Feature Selection: Selected features PT08.S1(CO), PT08.S2(NMHC), PT08.S3(NOx), PT08.S4(NO2), and PT08.S5(O3) to predict CO(GT).
Data Splitting: Split the data into training (80%) and testing (20%) sets.
Model Training: Trained a Linear Regression model on the training set.
Model Evaluation: Evaluated the model on the test set using Mean Squared Error (MSE) and R^2 Score.


6. Results
Mean Squared Error (MSE): [Insert MSE value]
R^2 Score: [Insert R^2 score]
Model Coefficients:
PT08.S1(CO): [Insert coefficient]
PT08.S2(NMHC): [Insert coefficient]
PT08.S3(NOx): [Insert coefficient]
PT08.S4(NO2): [Insert coefficient]
PT08.S5(O3): [Insert coefficient]
The R^2 score indicates how well the independent variables explain the variability of the dependent variable (CO(GT)). The coefficients provide insight into the relationship between each feature and the target variable.


7. Conclusion
The linear regression model provides a basic understanding of the relationships between CO concentration and other air quality sensors. While the model may not capture all complexities of the data, it offers a foundation for further analysis and improvement. Future steps could include exploring non-linear models or incorporating additional data for more robust predictions.
