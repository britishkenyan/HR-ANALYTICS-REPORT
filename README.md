# HR-ANALYTICS-REPORT
Here is a comprehensive report analyzing IBM HR Data to discover trends, challenges and insights about attrition within the company as well as recommend solutions. The dashboard focuses on exploring HR metrics and KPIs, with key focus on attrition rates, demographic insights and job satisfaction ratings.

----

### Contents (*click on the link to go directly to the page*)

[Project Overview](#project-overview)

[Data Sources](#data-sources)

[Tools Used](#tools-used)

[Data Cleaning and Preparations](#data-cleaning-and-preparations)

[Exploratory Data Analysis](#exploratory-data-analysis)

[Data Analysis](#data-analysis)

[Data Visualization](#data-visualization) 

[Data Visualization](#data-visualization) 

[Recommendations](#recommendations)

---

### Project Overview
This Data Analysis project aims to dive into IBM HR Data. The dashboard explores HR metrics and KPIs, with key focus on attrition rates, employee demographics, salary and job satisfaction ratings. The goal of this project is to analyze the HR data to identify trends and patterns that can help improve employee retention and inform HR strategies at IBM.

### Project Scope 
This analysis will explore the following:

- Employee Attrition: Understanding why employees leave and predicting the likelihood of attrition.
- Employee Performance: Analyzing factors that correlate with employee performance.
- Salary & Job Satisfaction: Investigating how these factors affect employee turnover and job satisfaction.

### Objective
The primary objective is to identify trends in employee turnover, determine the key factors influencing attrition, and provide recommendations for improving employee retention using Power BI’s analytical capabilities.
   
### Data Sources
The primary source of this dataset **hrdata.csv** is from open source platform Kaggle. The dataset contains information about employees, such as demographics, job role, salary, performance, and reasons for attrition - [download here] (https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
- Microsoft Excel - [Download Here] (https://www.microsoft.com) 

### Tools Used 
- Power BI: For data cleaning, analysis, visualization and dashboard creation.
- SQL (if applicable): For any additional preprocessing or querying.
- Excel/CSV: For data import and exploration.

### Data Collection and Preparation
Data Import: The data was imported into Power BI from the Kaggle dataset, typically in CSV format, using Power BI’s Get Data functionality. The dataset contains 1,470 rows and 35 columns. Key columns include the following:

- Employee Number: Unique identifier for each employee.
- Attrition: Whether the employee has left the company (Yes/No).
- Age: Age of the employee.
- JobRole: The role of the employee in the organization (e.g., Sales Executive, Research Scientist).
- DistanceFromHome: Distance of the employee’s home from the office.
- Performance Rating: Rating of employee performance.
- Education: Level of education attained by the employee.

Data Cleaning:
- Missing Values: Identified and handled any missing data, ensuring consistency across records.
- Data Type Correction: Ensured that all columns were in the correct data type (e.g., converting numerical columns to numeric types).
- Duplications: Checked for any duplicate rows and removed them.

Data Transformation: 
- Created additional columns where necessary, such as:
- Tenure: Based on the length of employment (can be derived from relevant columns like years).
- Job Satisfaction: A calculated measure of job satisfaction based on available data.
  
Data Model:
- Established relationships in Power BI between tables (e.g., linking the employee table to performance ratings or department details) to build a cohesive model for analysis.

### Exploratory Data Analysis (EDA)
Summary Statistics:
- Age: Mean age of employees, distribution of age across the company.
- Tenure: Length of employment across different job roles.
- Performance Ratings: Distribution of performance ratings and its relationship to attrition.
- Job Satisfactory Ratings:  Distribution of job satisfactory ratings and its relationship to attrition.
- Salary: Average salary by job role, and the distribution of salary in different departments.

**Visualizations**
Bar Charts:
- Distribution of Attrition by JobRole to see which departments experience the highest turnover.
- Salary Distribution for employees who stayed vs. those who left.

Pie Charts:
- Breakdown of Attrition by Gender, Department, and Education Level.

Box Plots:
- Visualize the relationship between Age and Attrition.

Heatmaps: Show correlation between numerical features like Distance From Home, Age, and Attrition.

---

### Dashboard Screenshot

---

### Analysis and Interpretation
**Key HR Metrics**
Attrition Rate: Percentage of employees leaving the company per department or job role.
Retention Rate: The rate at which employees stay over time.
Performance Impact: How performance ratings affect employee retention.
Salary Impact: Analyzing if higher salaries correlate with lower attrition.

**Advanced Analysis**
Predictive Analysis: Using Power BI’s machine learning features (e.g., Azure Machine Learning integration) to predict the likelihood of attrition based on historical data.
Clustering: Segmenting employees based on factors like age, salary, tenure, and performance to identify high-risk attrition groups.

Power BI Features Used:
DAX for creating calculated columns (e.g., turnover rate, performance score).
Power Query to clean and transform data (e.g., replacing null values, merging columns).
Custom Visuals for advanced visualizations like cluster maps or KPI indicators.

### Key Findings
Employee Demographics & Attrition:
Younger employees (under 30) exhibit higher attrition rates.
Employees in Sales and Research roles tend to leave more frequently than those in Engineering or HR.

Performance & Salary:
Higher performance ratings tend to reduce the likelihood of attrition.
Employees with higher salaries in managerial positions show lower turnover rates.

Trends over Time:
Attrition has spiked in recent years, suggesting potential dissatisfaction with recent company changes (e.g., policy, leadership).

Attrition:
High attrition in younger employees: Employees with less tenure, particularly in younger age groups, show higher attrition rates.
Sales and Research roles have higher turnover compared to other departments.
Performance Rating correlates with attrition, with lower performance ratings having higher turnover.

### Recommendations
Based on the analysis, here are some actionable recommendations for IBM HR as follows

- Increase Retention Among Young Employees: Implement mentorship programs and career development initiatives targeted at younger employees, especially those in Sales and Research.
- Address Performance Feedback: Provide more frequent and constructive feedback to employees with lower performance ratings to improve job satisfaction and reduce turnover.
- Salary Review: Conduct a salary review to ensure employees in high-turnover departments like Sales are compensated fairly compared to industry standards.
- Diversity and Inclusion Programs: Focus on promoting diversity, especially in high-turnover roles, and ensure that employee concerns regarding gender or age bias are addressed.

### Project Learnings

### Conclusion
This analysis provided valuable insights into IBM’s employee attrition patterns. The findings suggest that younger employees and certain job roles experience higher turnover rates. By implementing targeted retention strategies and adjusting performance management practices, IBM can reduce attrition and improve employee satisfaction.

*Future work could focus on a more detailed predictive model for attrition or investigating additional factors, such as company culture or external job market influences.*




<!--- #### Data Cleaning and Preparations
 During the initial phase of Data cleaning and preparation, we perform the following task
 1. Data Loading and Inspection
 2. Handling missing variables
 3. Data Cleaning and Formatting

#### Exploratory Data Analysis
EDA involves the exploration of data to answer key questions about data such as:
1. what is the overall sales trend?
2. What products are top sellers?
3. What are the products on peak sales?

<!---
IBM HR Analytics: Data Analysis Project Documentation
1. Overview
Introduction: The dataset you provided is focused on employee attrition within IBM, offering various HR metrics such as employee age, job role, salary, and performance ratings. The goal of this project is to analyze the HR data to identify trends and patterns that can help improve employee retention and inform HR strategies at IBM.

Project Scope: This analysis will explore:

Employee Attrition: Understanding why employees leave and predicting the likelihood of attrition.
Employee Performance: Analyzing factors that correlate with employee performance.
Salary & Job Satisfaction: Investigating how these factors affect employee turnover and job satisfaction.
Data Source: The dataset was sourced from Kaggle's IBM HR Analytics Attrition Dataset. The dataset contains information about employees, such as demographics, job role, salary, performance, and reasons for attrition.

Tools Used:

Power BI: For data visualization and dashboard creation.
SQL (if applicable): For any additional preprocessing or querying.
Excel/CSV: For data import and exploration.
Objective: The primary objective is to identify trends in employee turnover, determine the key factors influencing attrition, and provide recommendations for improving employee retention using Power BI’s analytical capabilities.

2. Data Collection and Preparation
Data Import: The data was imported into Power BI from the Kaggle dataset, typically in CSV format, using Power BI’s Get Data functionality. The dataset contains 1,470 rows and 35 columns. Key columns include:

EmployeeNumber: Unique identifier for each employee.
Attrition: Whether the employee has left the company (Yes/No).
Age: Age of the employee.
JobRole: The role of the employee in the organization (e.g., Sales Executive, Research Scientist).
DistanceFromHome: Distance of the employee’s home from the office.
PerformanceRating: Rating of employee performance.
Education: Level of education attained by the employee.
Data Cleaning:

Missing Values: Identified and handled any missing data, ensuring consistency across records.
Data Type Correction: Ensured that all columns were in the correct data type (e.g., converting numerical columns to numeric types).
Duplications: Checked for any duplicate rows and removed them.
Data Transformation:

Created additional columns where necessary, such as:
Tenure: Based on the length of employment (can be derived from relevant columns like years).
Job Satisfaction: A calculated measure of job satisfaction based on available data.
Data Model:

Established relationships in Power BI between tables (e.g., linking the employee table to performance ratings or department details) to build a cohesive model for analysis.
3. Exploratory Data Analysis (EDA)
Summary Statistics:

Age: Mean age of employees, distribution of age across the company.
Tenure: Length of employment across different job roles.
Performance Ratings: Distribution of performance ratings and its relationship to attrition.
Salary: Average salary by job role, and the distribution of salary in different departments.
Visualizations:

Bar Charts:
Distribution of Attrition by JobRole to see which departments experience the highest turnover.
Salary Distribution for employees who stayed vs. those who left.
Pie Charts:
Breakdown of Attrition by Gender, Department, and Education Level.
Box Plots:
Visualize the relationship between Age and Attrition.
Heatmaps: Show correlation between numerical features like DistanceFromHome, Age, and Attrition.
Key Insights:

High attrition in younger employees: Employees with less tenure, particularly in younger age groups, show higher attrition rates.
Sales and Research roles have higher turnover compared to other departments.
Performance Rating correlates with attrition, with lower performance ratings having higher turnover.
4. Analysis and Interpretation
Key HR Metrics:

Attrition Rate: Percentage of employees leaving the company per department or job role.
Retention Rate: The rate at which employees stay over time.
Performance Impact: How performance ratings affect employee retention.
Salary Impact: Analyzing if higher salaries correlate with lower attrition.
Advanced Analysis:

Predictive Analysis: Using Power BI’s machine learning features (e.g., Azure Machine Learning integration) to predict the likelihood of attrition based on historical data.
Clustering: Segmenting employees based on factors like age, salary, tenure, and performance to identify high-risk attrition groups.
Power BI Features Used:

DAX for creating calculated columns (e.g., turnover rate, performance score).
Power Query to clean and transform data (e.g., replacing null values, merging columns).
Custom Visuals for advanced visualizations like cluster maps or KPI indicators.
5. Key Findings
Employee Demographics & Attrition:
Younger employees (under 30) exhibit higher attrition rates.
Employees in Sales and Research roles tend to leave more frequently than those in Engineering or HR.
Performance & Salary:
Higher performance ratings tend to reduce the likelihood of attrition.
Employees with higher salaries in managerial positions show lower turnover rates.
Trends over Time:
Attrition has spiked in recent years, suggesting potential dissatisfaction with recent company changes (e.g., policy, leadership).
6. Recommendations
Based on the analysis, here are some actionable recommendations for IBM HR:

Increase Retention Among Young Employees: Implement mentorship programs and career development initiatives targeted at younger employees, especially those in Sales and Research.
Address Performance Feedback: Provide more frequent and constructive feedback to employees with lower performance ratings to improve job satisfaction and reduce turnover.
Salary Review: Conduct a salary review to ensure employees in high-turnover departments like Sales are compensated fairly compared to industry standards.
Diversity and Inclusion Programs: Focus on promoting diversity, especially in high-turnover roles, and ensure that employee concerns regarding gender or age bias are addressed.
7. Conclusion
This analysis provided valuable insights into IBM’s employee attrition patterns. The findings suggest that younger employees and certain job roles experience higher turnover rates. By implementing targeted retention strategies and adjusting performance management practices, IBM can reduce attrition and improve employee satisfaction.

Future work could focus on a more detailed predictive model for attrition or investigating additional factors, such as company culture or external job market influences.




<!---
####  Data Analysis
This is where we include basic lines of code or queries or even some DAX expression used during analysis

```SQL
SELECT * WILDCARD
WHERE AVG AGE >= 20
```
💻
|heading 1|heading 2|
------|------|
|table 1|table 2|


#### Data Visualization (Images)



####  Recommendations
