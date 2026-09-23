HR Capstone Dataset Analysis
📌 Project Overview

This project focuses on analyzing an HR employee dataset using Python and popular data analysis and visualization libraries.

The analysis starts with basic data exploration and cleaning, followed by visualization of important HR-related attributes such as:

Employee satisfaction level
Salary distribution
Department-wise employee count
Dataset structure and statistics
Missing values
Duplicate records

The project was developed in Jupyter Notebook as a beginner-friendly data analytics project.

🎯 Project Objectives

The main objectives of this project are:

Understand the structure of the HR dataset.
Explore the dataset using Pandas.
Check data types and statistical information.
Identify missing values.
Detect and remove duplicate records.
Analyze employee satisfaction levels.
Analyze employee salary categories.
Understand employee distribution across departments.
Create meaningful visualizations using Matplotlib and Seaborn.
🛠️ Technologies Used
Technology	Purpose
🐍 Python	Data analysis
🐼 Pandas	Data manipulation
🔢 NumPy	Numerical operations
📊 Matplotlib	Data visualization
📈 Seaborn	Statistical visualization
📓 Jupyter Notebook	Project development
📂 Project Structure
HR-Capstone-Data-Analysis/
│
├── HR_Capstone_Analysis.ipynb
├── HR_capstone_dataset.csv
└── README.md
🔍 Analysis Performed
1. Importing Libraries

The project uses:

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

These libraries are used for data loading, manipulation, numerical operations, and visualization.

2. Loading the Dataset

The HR dataset is loaded using Pandas:

df = pd.read_csv("HR_capstone_dataset.csv")

The dataset is then explored using:

df.head()
df.tail()
3. Dataset Exploration

Several commands are used to understand the dataset:

df.shape
df.dtypes
df.columns
df.describe()

These operations help understand:

Number of rows and columns
Data types
Available variables
Numerical statistics
4. Missing Value Analysis

Missing values are checked using:

df.isnull().sum()

This helps identify whether any columns contain missing data.

5. Duplicate Record Analysis

Duplicate records are identified using:

df.duplicated().sum()

Duplicate records are then removed:

df = df.drop_duplicates()

This improves the quality of the dataset before analysis.

📊 Exploratory Data Analysis
1. Employee Satisfaction Level

The project analyzes the distribution of employee satisfaction levels.

sns.histplot(
    df['satisfaction_level'],
    bins=20,
    kde=True
)

The visualization helps understand how employee satisfaction levels are distributed across the dataset.

Visualization

The project creates a histogram with a KDE curve to observe the overall distribution of satisfaction levels.

2. Salary Distribution

Salary categories are analyzed using:

df['salary'].value_counts()

A count plot is then created:

sns.countplot(
    x='salary',
    data=df
)

This provides a visual comparison of employees across different salary categories.

3. Department Analysis

The project also analyzes employee distribution across departments.

df['Department'].value_counts()

A horizontal count plot is used to visualize the number of employees in each department:

sns.countplot(
    y='Department',
    data=df,
    order=df['Department'].value_counts().index
)

This makes it easier to compare employee counts between departments.

📈 Key Areas Covered

The notebook currently focuses on:

✅ Data Loading
✅ Data Exploration
✅ Dataset Shape
✅ Column Information
✅ Data Types
✅ Descriptive Statistics
✅ Missing Value Checking
✅ Duplicate Detection
✅ Duplicate Removal
✅ Satisfaction Level Analysis
✅ Salary Analysis
✅ Department Analysis
✅ Data Visualization
🚀 How to Run the Project
Step 1: Clone the Repository
git clone https://github.com/abhishektyagi03/HR-Capstone-Data-Analysis.git
Step 2: Open the Project

Open the project folder in Jupyter Notebook or VS Code.

Step 3: Install Required Libraries
pip install pandas numpy matplotlib seaborn jupyter
Step 4: Start Jupyter Notebook
jupyter notebook
Step 5: Open the Notebook

Open:

HR_Capstone_Analysis.ipynb

Make sure the CSV dataset is available in the project directory.

💡 Skills Demonstrated

This project demonstrates practical knowledge of:

Python for Data Analysis
Pandas
NumPy
Exploratory Data Analysis (EDA)
Data Cleaning
Duplicate Handling
Statistical Summary
Data Visualization
Matplotlib
Seaborn
Jupyter Notebook
🔮 Future Improvements

The project can be extended with additional HR analytics such as:

Employee turnover/attrition analysis
Department-wise satisfaction analysis
Salary vs satisfaction analysis
Work-hours analysis
Promotion analysis
Employee performance analysis
Correlation analysis
Interactive Power BI dashboard
Employee attrition prediction using Machine Learning
👨‍💻 Author

Abhishek Tyagi

MCA | Aspiring Data Analyst / Data Scientist

Skills

Python SQL Excel Power BI Pandas NumPy Matplotlib Seaborn Data Analysis

⭐ Project

If you find this project useful, consider giving the repository a ⭐ on GitHub.
