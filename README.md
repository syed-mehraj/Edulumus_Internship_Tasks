Student Performance Analysis & Prediction
📘 Overview

This project is part of my Edulumus Internship, focusing on data analysis and machine learning using the Students Performance in Exams dataset from Kaggle.
The goal is to explore how demographic and socio-educational factors affect students’ academic performance and to build models that predict their exam scores.

🎯 Objectives

Perform Exploratory Data Analysis (EDA) to understand relationships between features like gender, ethnicity, lunch type, and parental education.

Visualize performance trends across various student groups.

Build regression models to predict math, reading, and writing scores.

Compare single-output and multi-output models for score prediction.

📊 Dataset Details

Source: Students Performance in Exams – Kaggle

Attributes:

Feature	Description
gender	Male / Female
race/ethnicity	Group A–E
parental level of education	Highest education of parent
lunch	Standard or free/reduced
test preparation course	Completed / None
math score	Out of 100
reading score	Out of 100
writing score	Out of 100
🔍 Exploratory Data Analysis

Compared average scores by gender, ethnicity, and lunch type.

Observed effect of test preparation courses on performance.

Used pairplots and boxplots to identify relationships among subjects.

Found that reading and writing scores are highly correlated.

🧠 Machine Learning Models
🔹 Single Output Regression

Predicted Math Score using:

LinearRegression with categorical encoding (OneHotEncoder)

Evaluation Metrics:

Mean Absolute Error (MAE)

R² Score

🔹 Multi Output Regression

Predicted Math, Reading, and Writing Scores together using:

RandomForestRegressor wrapped with MultiOutputRegressor

📈 Model Performance
Subject	MAE	RMSE	R²
Math	12.46	15.80	-0.026
Reading	11.89	15.21	-0.022
Writing	11.23	14.00	-0.018

🔹 Observation:
The low R² indicates that demographic data alone is insufficient to predict scores accurately — academic performance depends on additional unmeasured factors like motivation, study habits, and environment.

🧰 Tools & Libraries

Programming Language: Python

Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

Environment: Google Colab / VS Code

Version Control: Git & GitHub
