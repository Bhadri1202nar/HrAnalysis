# HrAnalysis

Power Bi Report link https://app.powerbi.com/groups/me/reports/4f025788-b17d-402e-afca-76adc92a202f/b17f3f084c0de37c6644?experience=power-bi
---

## HR Analytics Dashboard

### Problem Statement

This dashboard helps the HR department understand workforce demographics, attrition, and employee satisfaction levels. It provides insights into how different departments, age groups, education levels, and job roles are contributing to employee attrition. Additionally, it gives visibility into the job satisfaction ratings across various roles, allowing the company to focus on improving employee engagement and retention. By using this dashboard, the company can take targeted actions to reduce attrition, improve satisfaction, and ensure balanced workforce management.

---

### Steps Followed

- **Step 1:** Data was loaded into Power BI Desktop, likely sourced from an employee HR database. Key fields include department, age group, education, job role, and satisfaction ratings.
  
- **Step 2:** In Power Query Editor, under the "View" tab, "Column Distribution," "Column Quality," and "Column Profile" options were enabled to examine the data quality and distribution.
  
- **Step 3:** The dataset was profiled based on the entire dataset to ensure all rows were considered for analysis.

- **Step 4:** The dashboard visualizes employee information, attrition statistics, and satisfaction ratings using multiple charts and cards. Fields like "Department," "Age Group," "Job Role," and "Education" were used to categorize employees.

- **Step 5:** Multiple DAX measures were used to calculate values such as the attrition count, attrition rate, number of active employees, and average age. For example:
  - **Attrition Rate =** `(Count of employees who left / Total Employees) * 100`
  - **Active Employees =** `Total Employees - Attrition Count`
  
- **Step 6:** Filters were used to create visuals based on different dimensions like age group, gender, department, and education. The dashboard provides a breakdown of attrition and employee distribution across these fields.

- **Step 7:** A pie chart was used to represent department-wise attrition, helping identify which departments have the highest attrition rates.

- **Step 8:** A bar chart was created to show the number of employees by gender across different age groups. This visualizes how the workforce is distributed across age bands.

- **Step 9:** Another bar chart was used to represent job satisfaction ratings across various roles. The ratings are distributed from 1 to 5, with the total number of employees for each rating shown per job role.

- **Step 10:** Multiple donut charts were used to represent the attrition rate by gender and age group. This helps visualize the percentage of male vs. female attrition across different age bands.

- **Step 11:** A bar chart was added to show the number of employees who have left the company by education field, which gives insights into whether certain educational backgrounds have a higher risk of attrition.

- **Step 12:** Card visuals were used to display key metrics at a glance:
  - **Overall Employees:** 1470
  - **Attrition Count:** 237
  - **Attrition Rate:** 16.12%
  - **Active Employees:** 1233
  - **Average Age:** 37 years

- **Step 13:** Visual elements like themes and custom colors were applied to give the dashboard a cohesive look.

- **Step 14:** In the report view, text boxes were added to highlight key KPIs like attrition rate, number of employees, and average age.

---

### Insights

#### 1. Key Metrics
- **Overall Employees:** 1470 employees are represented in the dataset.
- **Attrition Count:** 237 employees have left the company.
- **Attrition Rate:** 16.12% of employees have left, which is a significant percentage.
- **Active Employees:** 1233 employees are currently active within the organization.
- **Average Age:** The average age of employees is 37 years, which gives insight into the workforce demographic.

#### 2. Department-wise Attrition
- **R&D Department:** 56.12% of the total attrition (133 employees).
- **Sales Department:** 38.8% of the attrition (92 employees).
- **HR Department:** 5.06% of the attrition (12 employees).
  - **Insight:** The R&D department faces the highest attrition rate, and strategies should be focused here to retain employees.

#### 3. Age Group Distribution
- The **25-34** age group has the largest number of employees, with a significant number of both female (217) and male (337) employees.
- The **45-54** and **Over 55** age groups have fewer employees, with minimal attrition.

#### 4. Education Field and Attrition
- **Life Sciences:** 89 employees have left, making it the field with the highest attrition rate.
- **Medical and Marketing Fields:** Also show significant attrition, with 63 and 35 employees leaving, respectively.
  - **Insight:** Life Sciences may require attention in terms of employee engagement or job satisfaction.

#### 5. Attrition by Age and Gender
- **Under 25:** 52.63% of female employees have left compared to 47.37% of males.
- **25-34:** Attrition is higher among females (61.6%) than males (38.39%).
- **35-44:** Attrition among females is 72.55%, significantly higher than males.
  - **Insight:** Female employees in younger age groups are more likely to leave, suggesting the need for targeted retention strategies.

#### 6. Job Satisfaction Rating
- **Healthcare Representative:** Most employees rate their job satisfaction at 3 or 4, suggesting room for improvement.
- **Research Scientist and Sales Executive:** These roles have relatively higher satisfaction scores, while **Human Resources** roles have a more even distribution of ratings.

---

### Additional Measures

1. **Total Number of Employees =** `COUNT(Employee[ID])`
   - Used to display the total number of employees on the dashboard.

2. **Attrition Rate (%) =** `(COUNT(Employee[Attrition]) / COUNT(Employee[ID])) * 100`
   - A custom measure was used to calculate the attrition rate for visualization.

3. **Active Employees =** `Total Employees - Attrition Count`
   - A measure for calculating how many employees are currently active.

---
###Final dashboard
<img width="521" alt="dashboard_snapshot" src="https://github.com/user-attachments/assets/36368fa9-be51-4ac6-970b-225f49a00a6a">

### Conclusion

This HR Analytics dashboard provides a comprehensive overview of employee demographics, attrition, and satisfaction, allowing for data-driven decision-making. Insights such as high attrition rates in specific departments or age groups help the HR team focus on retention strategies. Employee satisfaction ratings give a detailed view of areas needing improvement across different job roles.

The report was published to Power BI Service for wider access and regular updates.

---

