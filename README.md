# LITA_HR_DATA_ASSIGNMENT
This repository showcases my completion of an assignment given by my facilitator, demonstrating the knowledge and skills gained through the Power BI class. The project focuses on Human Resources Management.

### PROJECT TITLE: HUMAN RESOURCES DATA

[PROJECT OVERVIEW](#project-overview)

[DATA SOURCES](#data-sources)

[DATA DESCRIPTION](#data-description)

[TOOLS USED](#tools-used)

[DATA CLEANING AND PREPARATIONS](#data-cleaning-and-preparations)

[DATA TRANSFORMATION](#data-transformation)

[DATA ANALYSIS](#data-analysis)

[DATA VISUALIZATION](#data-visualization)

[INSIGHTS](#insights)

[RECOMMENDATIONS](#recommendations)

### PROJECT OVERVIEW
---
This project, which was part of the training conducted during the LITA Data Analysis class, presents the attrition rates of employee in an organization, The goal of the project was to address the issues of employee's attritons from the organization. Despite the organization"s activities of training, providing for and maintaining their staff, employees keep leaving the organization to other places. The analysis includes deriving various objectives, to understand better the underlying issues and to propose actionable recommendations that would reduce employee attritions from the organization.

### DATA SOURCES
---
Data used for this project was an excel data provided by the facilitators.

### DATA DESCRIPTION
---
The dataset includes the following fields:
1. Attrition: The Column tells us if the employees are still in the organization or not
2. Age Band: This shows the age groups of all the employees in the organization
3. Department : Department pf Employees
4. Gender: Gender of employees
5. Education Field: Educational field of employees
6. Job Role: Employee"s Job roles
7. Marital Status: Marital Status of staff
8. Employee Counts: Total Employee Counts
9. Job Level: Job Level
10. Attrition Counts: Cunts of thpse leaving the Organization
11. Attrition rates: rates at which they are leaving
12. Work Life Balance.

### TOOLS USED
---
1. Microsoft Excel [Download here](https://www.microsoft.com)
- For Data Input
- For Analysis
- For Data Cleaning
- For Data visualization
  
2. Microsoft SQL Server [Download here](https://www.microsoft.com/en-us/sql-server/sql-server-downloads?msockid=2b7beaf97efb6b170d9dfff87f1b6a9f)
- To manage and querry data
- Microsoft Power BI Download Here
- For Data Transformation
- Data modelling
- To Create reports and dashboards that are collections of visuals.
  
4. GitHub [Click here to sign up](https://github.com/)
- For Portfolio Building

### DATA CLEANING AND PREPARATIONS
---
During the initial phase of the data entry, the folowing actions were performed
1. Data quality was ensured by correcting any spelling errors, and addressing missing values.
2. Standardization: Used find and replace to standardize certain fields
3. Data import from Excel

### DATA TRANSFORMATION
Data was transformed to thoroughly clean, remove issues with data and increase column quality, column distribution and profile to 100%
1. Data Types and Formatting: This was done to ensure all data fields were assigned the correct data types, with numerical fields formatted as whole numbers, text as text and date fields set to date format.
2. Sorting: Sorted the dataset by the Date column to organize transactions chronologically.
3. Created New Columns: Added a new column to have more calculations like Revenue

### DATA ANALYSIS
---
Here are some lines of code, queries & some of the DAX expressions used during my analysis;

```
Attrition Rate = SUM('HR data'[Attrition Count]) /SUM('HR data'[Employee Count])
Average Age = AVERAGE('HR data'[Age])
Age Sort = Table.TransformColumnTypes(#"Added Conditional Column5",{{"Job Satisfaction rating", type text}})

``` 

### DATA VISUALIZATION
---

### INSIGHTS
---
•	The visual showed that:
i.	Average age of Staff in the company is 37 years, which shows that the organization have more younger staff than the elderly ones.
ii.	A total of 237 employees, which is 16% of the total employees, left the company over time. This shows that the organization lost 16% of their staff, in which resources like time and money were spent training. For such an amount of employee to leave the organization showed that they were greatly dissatisfied with the organization's policies of handling their staff. This explanation goes in line with the visuals, which showed that out of the 237-employee attrition count, a total of 66 employees were very dissatisfied with their jobs and 46 employees were dissatisfied with their jobs. This could be the reason why they left the organization
iii.	Attrition count by gender showed that a total of 150 male and 87 females left the organization during the period, probably because the organization's policies favours the females than the males.
iv.	Attrition based on Department showed that the attrition rate was highest in Life Science department, which had a total of 89 staff that left the company, followed by the Medical department with a total of 63 attrition counts. Human resource had the lowest attrition rate, with a count of 7 employee who left the organization.
v.	Laboratory Technicians had the highest counts of very dissatisfaction rates, probably the reason why the Life science and medical field had the highest attrition rate compared to another department.
vi.	Attrition based on age groups showed that age group 25-34 had the highest attrition count, which showed that the younger people were more dissatisfied with the organizational policies.

### RECOMMENDATION
---
The followings were recommended based on findings from the Data Analysis, which enabled us took informed decisions such as:
1.	Policies should be amended: The Organization should amend their policies to favour all age groups and gender. The Executives should work on providing extracurricular activities like fitness coach or even work in line with a fitness Centre where their staff could enroll at a cheap rate for weekly fitness training, which would encourage more younger age groups to be satisfied and have great work like balance. All genders and age groups should be considered when allocating benefits or incentives
2.	Sisters Companies should be researched: The HR department should work on researching on how other sister's companies with similar goals and objectives treats their employees, so they can work on satisfying their staff
3.	Budget should be allocated to departments based on activities they have in line to do; this would reduce the number of unsatisfied staffs by departments
4.	All departments should be treated fairly
