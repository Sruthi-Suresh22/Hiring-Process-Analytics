# HIRING PROCESS ANALYTICS

## Table of Contents

- [Project Description](#project-description)
- [Dataset Details](#dataset-details)
- [Data Cleaning](#data-cleaning)
- [Data Analytics Tasks](#data-analytics-tasks)
- [Insights](#insights)
- [Conclusion](#conclusion)

## Project Description

The hiring process is a crucial function of any company, and understanding trends such as the number of rejections, interviews, job types, and vacancies can provide valuable insights for the hiring department. The goal of this project is to use the knowledge of statistics and Excel to draw meaningful conclusions about the company's hiring process. As a data analyst at a multinational company like Google, the task is to analyze the company's hiring process data and draw meaningful insights from it. The insights gained could potentially help the company improve its hiring process and make better hiring decisions in the future.

## Dataset Details

The Dataset **Statistics.xlsx** consists of 7,168 records with the following details:
- `application_id` : ID of the Applicant
- `Interview Taken on` : Interview Date and Time
- `Status` : Give details about whether an applicant is Hired or Rejected
- `event_name` : Gender of the Applicant
- `Department` : Name of the department for which the interview was conducted
- `Post Name` : Name of the Post
- `Offered Salary` : Salary offered for the particular post

## Data Cleaning

**1. Handling Missing Data:**

- `Offered Salary` column has **1** record with **blank** value which has the corresponding `Department column` as “**Sales Department**” and `Post Name` column as “**i7**”. This was replaced by the value **45400** obtained as the median of Offered Salary for Sales Department and Post Name as i7.
- `Post Name` column has **1** record with ‘**-**’ value which has the corresponding `Department` column as “**Sales Department**” and `Offered Salary` column as “**85914**”. This was replaced by the value **c9** obtained as the most commonly occurring Post Name while considering Sales Department and Offered Salary in the range of 85000 to 86000.
- There were **15** records having ‘**-**’ value in the `event_name` column. This was replaced by “**Don’t want to say**”.

**2. Error Correction:**

- In the column `Post Name`, all the values given as “**c-10**” which could be possibly due to human error was replaced with **c10** similar to other values.

**3. Handling Outliers:**

- While considering the `Offered Salary` column, there were 3 outliers **200000**, **300000**, and **400000** as determined from the **Scatter Plot**.
- These 3 values : 200000, 300000 and 400000 were replaced by the values **45039**, **57870** and **46134** respectively obtained by taking the median corresponding to the Department and Post Name.
  
![h1](https://github.com/Sruthi-Suresh22/Hiring-Process-Analytics/assets/162356465/4ea2c8f1-ed18-4cfd-9f8b-fbeb38bffd25)

## Data Analytics Tasks:

**A. Hiring Analysis:** The hiring process involves bringing new individuals into the organization for various roles.

*Task:* Determine the gender distribution of hires. How many males and females have been hired by the company?

**B. Salary Analysis:** The average salary is calculated by adding up the salaries of a group of employees and then dividing the total by the number of employees.

*Task:* What is the average salary offered by this company? Use Excel functions to calculate this.

**C. Salary Distribution:** Class intervals represent ranges of values, in this case, salary ranges. The class interval is the difference between the upper and lower limits of a class.

*Task:* Create class intervals for the salaries in the company. This will help you understand the salary distribution.

**D. Departmental Analysis:** Visualizing data through charts and plots is a crucial part of data analysis.

*Task:* Use a pie chart, bar graph, or any other suitable visualization to show the proportion of people working in different departments.

**E. Position Tier Analysis:** Different positions within a company often have different tiers or levels.

*Task:* Use a chart or graph to represent the different position tiers within the company. This will help you understand the distribution of positions across different tiers.

## Insights

**A. Hiring Analysis:**

![h2](https://github.com/Sruthi-Suresh22/Hiring-Process-Analytics/assets/162356465/1db18249-960c-40af-9578-56c74b30f899)

- From this analysis, we can understand that more than half of the employees hired are males, contributing 55% whereas the hired female population is about 39%.
- About 6% of the total hired employees have not disclosed their gender.
- This analysis helps the company to keep their focus more on maintaining gender equality by hiring accordingly so that their Gender ratio remains intact for an ideal workplace.

**B. Salary Analysis:**

![h3a](https://github.com/Sruthi-Suresh22/Hiring-Process-Analytics/assets/162356465/5752d009-67d8-4607-9f45-57c16e4e5a9f)
![h3b](https://github.com/Sruthi-Suresh22/Hiring-Process-Analytics/assets/162356465/efaa701c-2ac1-45ef-aab1-57d21059b8fd)

- The **Average salary** for hired candidates is found to be **currency unit 49593.02**.
- The department having the highest Average salary is “**General Management**”.

**C. Salary Distribution:**

![h4](https://github.com/Sruthi-Suresh22/Hiring-Process-Analytics/assets/162356465/99814904-4610-4830-86a5-24268ca07df6)

- Most of the employees are receiving salary in the range **40001-50000**, **500001-60000** which corresponds to average salary given to the hired candidates by the company.
- Almost there is an equal distribution of  employees from fresher to mid -senior to senior levels.

**D. Departmental Analysis:**

![h5](https://github.com/Sruthi-Suresh22/Hiring-Process-Analytics/assets/162356465/27fbae3a-c2f2-42c7-98e9-260cda1a67ac)

- **Operations Department** has the **highest** number of employees **1843** in number contributing **39.2%** of the total employees followed by **Service Department** contributing **28.4%** with **1332** employees.
- **Least** number of employees are present in the **Human Resource Department** with **70** employees.

**E. Position Tier Analysis:**

![h6](https://github.com/Sruthi-Suresh22/Hiring-Process-Analytics/assets/162356465/cf02fa12-12c4-4169-a5b6-ef3dd36d27a7)

- We can observe that the Company has hired **most candidates** for **c9** post-tier followed by **c5** and **i7**.
- **Least number of employees** are hired for **n6** and **m6**. 
- There are no employees hired for n10, m7 and n9 post tiers.

## Conclusion

The Hiring Process Analytics project have helped in understanding the concept of Exploratory Data Analysis and pivot tables along with using some of functions in MS Excel. By understanding more on the insights gained from this analysis such as hiring patterns, salary distribution and department-wise composition, the company can focus more the strategies to be taken during the recruitment process and also in promoting organizational growth.



  
