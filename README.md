# data-cleaning-with-pyspark

*COMPANY:CODTECH IT SOLUTIONS

#NAME:VIKAS R

#INTERN ID:CT06DH742

#DOMAIN:BIG DATA

#DURATION:6 WEEKS

#MENTOR:NEELA SANTHOSH

📌 Overview
This project demonstrates data cleaning using PySpark on the famous Wine dataset. The Wine dataset contains measurements of various chemical properties of wines along with their class labels.
In real-world scenarios, raw data often contains duplicates, missing values, and outliers that can impact the performance of data analysis or machine learning models.

This project simulates such issues, then applies data preprocessing techniques using PySpark to create a clean, analysis-ready dataset.

🎯 Objective
The main objective is to:

Load and explore the Wine dataset.

Introduce intentional data issues (missing values, duplicates) to mimic real-world problems.

Apply PySpark-based data cleaning techniques.

Save the cleaned dataset for further analysis or modeling.

📂 Dataset
We use the Wine dataset from the sklearn.datasets module.

Source: Scikit-learn Wine Dataset Documentation

Features: 13 numeric chemical analysis attributes (e.g., alcohol content, malic acid, color intensity).

Target: Class label indicating wine type (0, 1, or 2).

🛠 Technologies Used
Python 3.x

PySpark for big data processing

Pandas for initial dataset manipulation

Scikit-learn for dataset loading

NumPy for numeric operations

🧹 Data Cleaning Steps
Data Loading

Loaded the Wine dataset from Scikit-learn.

Converted to Pandas DataFrame for initial manipulation.

Introducing Data Issues (for demo purposes)

Added missing values in selected columns.

Added duplicate rows.

Reading into PySpark

Used spark.read.csv() to load the CSV into a Spark DataFrame.

Duplicate Removal

Used dropDuplicates() to remove duplicate rows.

Handling Missing Values

Calculated the mean for numeric columns using mean() from PySpark SQL functions.

Filled missing numeric values with corresponding mean values using na.fill().

Outlier Removal

Applied filters to remove unrealistic values (e.g., alcohol outside the range 0–20).

Saving Cleaned Data

Saved the cleaned DataFrame to a CSV file for future use.

📊 Results
Before Cleaning: Dataset contained duplicates and missing values.

After Cleaning:

All duplicates removed.

Missing numeric values replaced with column means.

Outliers removed.

Dataset ready for analysis or modeling.
