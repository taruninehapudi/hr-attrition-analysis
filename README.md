# hr-attrition-analysis
Project Overview

This project examines employee attrition patterns using the IBM HR dataset. The analysis includes exploratory data analysis (EDA), feature evaluation, and predictive modeling to understand the major factors driving employee turnover. The goal is to help organizations identify risk indicators and improve retention strategies.

Objectives

• Analyze demographic and job-related variables
• Identify trends and patterns linked to employee attrition
• Build classification models to predict likelihood of attrition
• Provide data-driven business recommendations

Tools Used

• Python
• Pandas
• NumPy
• Matplotlib
• Seaborn
• Scikit-learn
• Jupyter Notebook

Files in This Repository

• hr_attrition.ipynb — Main notebook for analysis and modeling
• sample_hr_attrition.csv — 10–20 row sample dataset for demonstration
• README.md — Project documentation

Dataset Source

The original dataset is publicly available on Kaggle:
https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset

Important Note (File Path Change Required)

In the original notebook, the dataset was loaded using a local system path such as:

data = pd.read_csv(r'D:\\Teks 2024\\HR-Employee-Attrition.csv')


Since this path will not work for other users or GitHub execution,
please replace it with:

data = pd.read_csv("sample_hr_attrition.csv")


This ensures the notebook runs correctly inside GitHub or on any other system.

Key Insights

• Employees with lower monthly income have higher attrition
• Overtime strongly increases attrition probability
• Job satisfaction and work-life balance are major influencing factors
• Attrition is higher among early-career and low-tenure employees

Modeling Summary

• Logistic Regression, Decision Tree, and Random Forest models were tested
• Random Forest gave the best performance
• Top predictors included overtime, income, job satisfaction, and age

Business Recommendations

• Reduce excessive overtime in high-risk departments
• Improve compensation for low-income employee segments
• Focus retention efforts on employees with low job satisfaction
• Implement early-warning indicators for employees at high attrition risk

How to Run This Project

Clone or download this repository

Keep sample_hr_attrition.csv in the same folder as the notebook

Open hr_attrition.ipynb using Jupyter Notebook

Ensure the file path inside the notebook uses:
data = pd.read_csv("sample_hr_attrition.csv")

Run all cells sequentially
