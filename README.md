# Salaries-san-francisco-employee

SALARIES ANALYSIS OF SAN FRANCISCO EMPLOYEES (2011 TO 2018)

PROJECT OVERVIEW

This project explores public employee salary data from the city of San Francisco, covering the years 2011 through 2018. The dataset contains more than 300,000 records and includes information on base pay, overtime, other types of pay, and benefits. The purpose of this analysis is to extract insights about salary trends, evaluate the distribution of compensation, and build a predictive model to estimate total pay including benefits.

The project is designed from the perspective of a finance analyst using tools like Python, Pandas, Seaborn, and Scikit-learn. It applies a structured approach that includes data cleaning, exploratory analysis, visualization, and basic machine learning modeling.


---

OBJECTIVES

Understand the structure of compensation for public employees.

Identify job titles with the highest total compensation.

Analyze salary trends over time.

Explore how different components like overtime pay and benefits affect total earnings.

Build a regression model to predict total pay benefits based on various inputs.



---

TOOLS USED

Python (Pandas, NumPy, Matplotlib, Seaborn)

Jupyter Notebook or Visual Studio Code

Scikit-learn (for regression modeling)



---

DATA DESCRIPTION

The dataset includes the following key columns:

EmployeeName: Full name of the employee

JobTitle: Job designation or role

BasePay: Base salary

OvertimePay: Additional pay for overtime work

OtherPay: Other forms of compensation

Benefits: Value of benefits provided

TotalPay: Total of base pay, overtime, and other pay

TotalPayBenefits: Total pay including benefits

Year: Payroll year (from 2011 to 2018)



---

DATA CLEANING

The raw dataset required several cleaning steps:

1. Data Type Conversion: Monetary columns were initially stored as strings. These were converted into numerical types.


2. Missing Values: Rows with missing critical salary values (especially BasePay and TotalPayBenefits) were dropped.


3. Outliers and Invalid Entries: Entries with negative pay values were filtered out as these likely represent data entry errors.



After cleaning, the dataset contained approximately 312,000 valid salary records.


---

EXPLORATORY DATA ANALYSIS

DISTRIBUTION OF PAY COMPONENTS

Histograms were plotted for BasePay, OvertimePay, and OtherPay. These distributions revealed that while most employees earned a moderate base salary, a small number of individuals received disproportionately high overtime or other types of pay.

TOP 10 HIGHEST PAYING JOB TITLES

By calculating the average TotalPay for each job title, we identified the most lucrative roles in the public sector. Executive and senior-level positions, particularly those in transit and public safety, consistently ranked among the highest.

SALARY TRENDS OVER TIME

A line chart of average TotalPay by year revealed a steady upward trend in compensation between 2011 and 2018, reflecting either increased public spending or inflation-adjusted pay increases.

CORRELATION ANALYSIS

A correlation matrix showed that:

BasePay and TotalPay are highly correlated.

Benefits contribute significantly to TotalPayBenefits.

There is moderate correlation between OvertimePay and overall compensation.



---

INDIVIDUAL ANALYSIS

An individual case study was conducted for Ricardo Jimenez, a Transit Supervisor. His yearly compensation from 2012 to 2018 showed consistent increases in both base pay and total compensation, with a peak in 2017.


---

SALARY DISTRIBUTION BY YEAR

Using grouped bar charts, we observed that:

The highest average base pay was recorded in 2018.

The number of unique job titles fluctuated slightly over the years, with the highest diversity in 2013.



---

MACHINE LEARNING MODELING

DATA PREPROCESSING

Categorical variables like JobTitle were converted to numerical format using one-hot encoding.

Features were separated from the target variable TotalPayBenefits.


MODEL TRAINING

A Linear Regression model was trained using Scikit-learn. The features included:

BasePay

OvertimePay

OtherPay

JobTitle (encoded)

Benefits


MODEL EVALUATION

The model's performance was evaluated using:

Mean Absolute Error (MAE): Measures average prediction error in salary units.

R-Squared Score: Measures the percentage of variation explained by the model.


While the model provided a reasonable baseline for predictions, results could be improved using more advanced techniques such as Random Forest or Gradient Boosting.


---

KEY INSIGHTS

The role of Chief Executive Officer and other senior management positions had the highest pay.

Transit Operators were among the most common job titles.

Pay levels have increased over the years, especially from 2015 onward.

A small group of employees receives unusually high levels of overtime and other pay.

Benefits are a major contributor to total compensation and should not be overlooked in compensation planning.



---

CONCLUSION

This project provided valuable insights into public sector compensation in San Francisco. By combining statistical analysis with visualization and regression modeling, we gained a clear understanding of how different factors influence employee pay.

The results can support budgeting, HR planning, and policy discussions. With further refinement, predictive models could help forecast future salary trends and detect anomalies in public payroll data.
