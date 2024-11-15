# HR Employee Data
---

## Table of Contents
[Project Overview](#project-overview)

[Data Used](#data-used)

[Tools Used](#tools-used)

[Data Cleaning and Preparation](#data-cleaning-and-preparation)

[Exploratory Data Analysis](#exploratory-data-analysis)

[Data Analysis Expression Function](#data-analysis-expression-function)

[Data Visualization](#data-visualization)

[Results and Insights](#results-and-insights)

[Conclusion](#conclusion)

[Recommendations](#recommendations)


### Project Overview
---
In this project, I conducted an in-depth analysis of HR Employee data to provide actionable insights that drive business decisions. The objective was to explore key metrics such as the number of attrition, attrition rate, attrition count by department, gender, educational field, age group, and job ratings based on attrition, culminating in an interactive Power BI dashboard. 

### Data used:
---
The dataset used for this analysis is the **"HR Data.xlsx"** file  provided by the _Ladies in Tech Africa Data Analysis Program_. For more info see [The Incubator Hub](https://www.theincubatorng.org/). It contains detailed information about each employee comprising 41 columns. The key columns are;

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
---
- **Power BI**: This visualizes the findings through interactive dashboards.

### Data Cleaning and Preparation
---
In the initial data preparation phase, I performed the following tasks:
1. Data loading and inspection.
2. Handling missing variables.
3. Data cleaning and formatting.

### Exploratory Data Analysis
---
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
---
- **Attrition Rate**
  ```DAX
   = SUM('HR data'[Attrition Count])/SUM('HR data'[Employee Count])
  ```

- **Average Age**
```DAX
= AVERAGE('HR data'[Age])
```

### Data Visualization
---

![HR Data Analysis Dashboard](https://github.com/Putsim/LITA_HR_Analysis/blob/main/HR%20data%20PBI.png)

![HR Data Analysis Dashboard](https://github.com/Putsim/LITA_HR_Analysis/blob/main/HR%20data%20contd%20PBI.png)

## Results and Insights
---
- **Overall Workforce and Attrition**:
  - **Total Employees**: 1,470.
  - **Attrition Count**: 237 employees, resulting in an **attrition rate of 16%**.
  - **Current Employees**: 1,233, with **501 females** and **732 males**.

- **Attrition by Gender and Age Group**:
  - **Gender**:
    - Male attrition: 150.
    - Female attrition: 87.
  - **Age Group**:
    - Highest attrition: **25-34 age group** with 112 employees.
    - Lowest attrition: **55+ age group** with 11 employees.

- **Attrition by Department**:
  - **R&D** department has the highest attrition rate at **56%**.
  - **HR** department has the lowest attrition rate at **5%**.

- **Attrition by Educational Field**:
  - Top 3 fields with the highest attrition: **Life Science, Medical, and Marketing**.
  - **HR** has the lowest attrition in educational field categories.

- **Job Roles and Attrition Rate**:
  - **Lab Technician** role has the highest attrition rate at **24%**, indicating possible job dissatisfaction.
  - Other notable job roles with high attrition rates:
    - **Sales Representatives**: 40%.
    - **Sales Executives**: 17%.
    - **Research Scientists**: 16%.

- **Job Satisfaction by Educational Field**:
  - **Life Science** shows the highest job dissatisfaction rate at **28%**, based on attrition.

- **Current Employee Insights by Marital Status and Gender**:
  - **Married males** constitute the largest group of current employees with **348 individuals**.


| Job Role               | Total Number of Attrition | Female | Male | Department | Attrition Rate | Average Age |
|------------------------|--------------------------|--------|------|------------|----------------|-------------|
| Healthcare             | 9                        | 5      | 4    | R&D        | 7%             | 40          |
| HR                     | 12                       | 6      | 6    | HR         | 23%            | 36          |
| Lab Technician         | 62                       | 16     | 46   | R&D        | 24%            | 34          |
| Manager                | 5                        | 2      | 3    | R&D        | 5%             | 47          |
| Manufacturing Director | 10                       | 4      | 6    | R&D        | 7%             | 38          |
| Research Director      | 2                        | 1      | 1    | R&D        | 3%             | 44          |
| Research Scientist     | 47                       | 17     | 30   | R&D        | 16%            | 34          |
| Sales Executives       | 57                       | 20     | 37   | Sales      | 17%            | 37          |
| Sales Representatives  | 33                       | 16     | 17   | Sales      | 40%            | 30          |


These findings reveal areas for potential improvement in employee retention, particularly in specific job roles, departments, and age groups where attrition and dissatisfaction are higher.


### Conclusion
---
The **overall attrition rate of 16%** is largely driven by the **R&D department** and roles like **Lab Technicians and Sales Representatives**, indicating specific areas of job dissatisfaction. The **25-34 age group** has the highest attrition rate, which may suggest issues with career development or job satisfaction for early-career employees. Gender-based attrition skews toward males, while **Life Science** as an educational field shows significant job dissatisfaction at 28%. High attrition within certain fields and age groups highlights key areas that need attention to improve employee retention and satisfaction.

### Recommendations
---
1. **Targeted Retention Strategies**:
   - Address job satisfaction concerns among **Lab Technicians and Sales Representatives** by improving job conditions, providing clearer career growth paths, and possibly increasing engagement initiatives.
2. **Career Development for Younger Employees**:
   - Implement mentorship and development programs specifically for the **25-34 age group** to encourage career growth and reduce attrition in this demographic.
3. **Focus on R&D Department Engagement**:
   - Investigate and address the factors contributing to the **56% attrition rate** in R&D through employee feedback and enhanced support for work-life balance.
4. **Tailored Programs by Educational Field**:
   - Improve satisfaction for employees from **Life Science** and **Medical fields** by offering role-specific training and support programs to reduce dissatisfaction and enhance their job experience.

These recommendations aim to improve employee engagement and retention, particularly within high-turnover groups and roles, leading to a more stable and satisfied workforce.
