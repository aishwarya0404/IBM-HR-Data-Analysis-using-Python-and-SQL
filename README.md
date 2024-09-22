# IBM-HR-Data-Analysis-using-Python-and-SQL

Overview
This project focuses on analyzing and predicting employee attrition within a company. By importing HR data from CSV files into a MySQL database, we can perform comprehensive data analysis to identify patterns and trends. The analysis leverages various statistical methods and machine learning algorithms, specifically logistic regression, to predict whether employees are likely to leave the company.

Through visualizations and descriptive statistics, the project aims to provide insights into factors influencing attrition, such as job role, age, and monthly income. This understanding can aid organizations in making informed decisions to enhance employee retention.

Dataset
The dataset is attached in a CSV file- . It includes various attributes related to employee demographics, job roles, compensation, and attrition status.

Installation
Ensure you have Python installed (preferably 3.7 or later).

Install the required packages using pip:

pip install pandas mysql-connector-python seaborn matplotlib scikit-learn
Set up a MySQL server and create a database named ibm.

Usage
Place your CSV files in the specified folder.
Update the CSV file names and corresponding table names in the script.
Run the Python script to import the data, analyze it, visualize it, and train the logistic regression model.
Data Import
The script reads specified CSV files and imports them into the MySQL database:

CSV files are read into Pandas DataFrames.
NaN values are replaced with None for SQL compatibility.
Column names are sanitized to fit SQL naming conventions.
A corresponding table is created in the database if it does not already exist.
Data Analysis
The data is analyzed to identify trends, such as the average monthly income by job role. Key numeric and categorical columns are separated for further analysis.

Data Visualization
Visualizations are created using Seaborn and Matplotlib:

Count plots for employee attrition.
Histograms for numeric variables.
Scatter plots to examine the relationship between age and monthly income.
Model Training
Logistic regression is used to predict employee attrition:

The features are standardized using StandardScaler.
The model is trained on the training dataset and evaluated on the test dataset.
Results
The performance of the logistic regression model is evaluated using a confusion matrix and classification report. Key metrics include precision, recall, and F1-score.
