# LITA_HR_Analysis
This project demonstrates my ability to analyze and derive actionable insights from HR data using Power BI. The objective was to explore factors influencing attrition, understand employee satisfaction, and identify trends in performance and compensation across different age groups, education fields, or job roles.

# HR Employee Data
---
### Project Overview
In this project, I conducted an in-depth analysis of HR Employee data to provide actionable insights that drive business decisions. The objective was to explore key metrics such as the number of attrition, attrition rate, attrition count by department, gender, educational field, age group, and job ratings based on attrition, culminating in an interactive Power BI dashboard. 

### Data used:
The dataset used for this analysis is the **"HR Data.xlsx"** file, containing detailed information about each employee. It comprises of 41 columns. The key columns are;

1. **Attrition**: Indicates whether the employee is still with the company ("No") or has left ("Yes").
2. **Business Travel**: Specifies the frequency of business travel (e.g., "Travel_Rarely," "Travel_Frequently").
3. **Age Band**: Groups employees by age ranges (e.g., "25-34," "35-44").
4. **Attrition Label:** Classifies employees as "Current Employees" or "Ex-Employees."
5. **Department:** Specifies the department (e.g., "Sales," "R&D").
6. **Education Field:** Shows the field of education (e.g., "Life Sciences," "Medical").
7. **Employee Number/emp no:** Unique identifier for each employee.
8. **Gender and Job Role:** Includes gender and specific job role (e.g., "Laboratory Technician," "Research Scientist").
9. **Marital Status and Over Time:** Shows marital status (e.g., "Single," "Married") and whether the employee works overtime.
10. **Training Times Last Year:** Indicates the number of training sessions attended in the past year.
11. **Age and Daily Rate:** Shows the age of employees and their daily pay rate.
12. **Distance From Home:** This represents the distance the employee lives from the workplace.
13. **Education, Job Level, and Job Satisfaction:** Includes education level, job involvement, and satisfaction levels.
14. **Monthly Income and Percent Salary Hike:** Displays monthly earnings and recent percentage salary increases.
15. **Performance Rating and Work-Life Balance:** Assesses performance and work-life balance levels.
16. **Years of Experience and Manager Relationship:** Tracks years at the company, with the current manager, and years since the last promotion.

### Tools Used:
- **Power BI**: This visualizes the findings through interactive dashboards.

### Data Cleaning/ Preparation
In the initial data preparation phase, I performed the following tasks:
1. Data loading and inspection.
2. Handling missing variables.
3. Data cleaning and formatting.

### Exploratory Data Analysis
In this project, I translated these findings into a user-friendly and interactive dashboard with these key metrics.
- Number of Attrition.
- Attrition rate.
- Attrition count by department,
- Attrition count by educational field
- Attrition count by gender
- Attrition count by age group
- Job rating based on attrition
- Job satisfaction by educational field based on attrition
- Current employee by marital status and gender
- Current employee based on age group and gender
- Attrition based on age group and gender
  
### Data Analysis Expression Function
- **Attrition Rate**
  ```DAX
   = SUM('HR data'[Attrition Count])/SUM('HR data'[Employee Count])
  ```

- **Average Age**
```DAX
= AVERAGE('HR data'[Age])
```

### Data Visualization

![HR Data Analysis Dashboard](https://github.com/Putsim/LITA_HR_Analysis/blob/main/HR%20data%20PBI.png)

![HR Data Analysis Dashboard](https://github.com/Putsim/LITA_HR_Analysis/blob/main/HR%20data%20contd%20PBI.png)


