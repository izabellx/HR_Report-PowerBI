# HR Report

## Problem Statement 

This project utilizes Power BI to create a comprehensive HR analytics report. The report is designed to provide detailed 
insights into various aspects of human resource management, including employee demographics, divercity policies and pay equity. 

### Steps Followed

 - Step 1 : Download the Data from Kaggle
 - Step 2 : Upload the Data to Excel
 - Step 3 : Data Cleaning (used: Find&Replace, Remove Duplicates, Spelling, Format of Data, Trim() function)
 - Step 4 : Upload the clean Data to Power Bi
 - Step 5 : Transform Data Look for errors or empty values. 
 - Step 6 : Check format of Data
 - Step 7 : Upload 2nd table to Power Bi.
 - Step 8 : Check if Date format is correct.
 - Step 9 : Create connection in model.

     ![model](https://github.com/user-attachments/assets/ca7fde4b-0fb4-4f50-a4f4-8008ed363c36)

 - Step 10 : Create measures for Average Salary, Headcount, Male Employees, %Male Employees, Female Employees, %Female Employees:

        % Female Employees = DIVIDE([Female Employees, [Headcount])

        % Male Employee = DIVIDE([Male Employees], [Headcount])

        Average Salary = AVERAGE(hrdataset[Salary])

        Female Employees = CALCULATE(COUNT(hrdataset[EmpID]), hrdataset[Sex] = "Female")

        Male Employees = CALCULATE(COUNT(hrdataset[EmpID]), hrdataset[Sex] = "Male")

        Headcount = COUNT(hrdataset[EmpID])


 - Step 11 : Add shapes, title of the Employee Demographics dashboard.
 - Step 12 : Add KPIs : Headcount, Male Employees, %Male Employees, Female Employees, %Female Employees.

    ![KPI1](https://github.com/user-attachments/assets/b77ff0e0-e6ca-48ac-8849-ed086becdd2a)

 - Step 13 : Add bar charts Employee by Race, Marital Status, Department.
 - Step 14 : Create Age Groups ("Age(bins)").
 - Step 15 : Add column chart Employees by Age Groups.
 - Step 16 : Insert map to visualize the States where employees live.
 - Step 17 : Insert dropdown slicers - Race, Department and Position.
 - Step 18 : Duplicate Dashboard.
 - Step 19 : Rename to "Salary and Compensation"
 - Step 20 : Add navigation buttons.
 - Step 21 : Add KPIs : Average Salary, Median Salary, Min Salary, Max Salary.
 
![KPI2](https://github.com/user-attachments/assets/9645afdb-b210-4c2c-8ad1-c394088e6562)

 - Step 22 : Insert bar chart Average Salary by Department, donut chart Average Salary by Gender.
 - Step 23 : Insert table, filter 10 top employees.
 - Step 24 : Add colum chart Average Salary by Race.
 - Step 25 : Insert dropdown slicers - Race, Performance.


# Report

![Dashboard0](https://github.com/user-attachments/assets/0a388e7e-f04a-4003-8a85-a14e0f72e3be)
![Dashboard1](https://github.com/user-attachments/assets/e2f342fc-6c7e-49e6-9c21-5fbcd5d31c72)
![Dashboard2](https://github.com/user-attachments/assets/8a118364-9d84-4634-8230-4f4b9e5e7156)

# Insights

Following interferences can be drawn from the report:

### [1] Gender Representation:

	The company has a higher percentage of female employees (57%) compared to male employees (43%).

### [2] Race Representation:

	The workforce is predominantly White, with Black employees being the second most represented race. 
	There is a noticeable underrepresentation of Asian, Indian, and Hispanic employees.

### [3] Age Distribution: 

	Most employees are in their 30s, which could indicate a relatively young workforce with potential for growth 
	and career development.

### [4] Salary Disparities:
	
	Significant salary disparity between departments, with Executive Office and IT/IS departments having higher average salaries.
	Gender pay gap exists but is relatively small.
	There are racial disparities in average salary, with Indian and White employees earning more on average compared 
	to other races.

### [5] High Earners: 

	The top earners are primarily in leadership and IT roles, reflecting the high value placed on these positions 
	within the company.
