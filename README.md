# DSA-Palmora-Group-HR-Analysis-Project

This repository contains information on the data Analysisnproject developed using Power BI. the project focuses on specific domains and provides visualization, insights and analytics based on the dataset


## PROJECT TOPIC: Palmora Group HR Analysis  


### PROJECT OVERVIEW: 
This Data Analysis project aims to analyze in issues bordering on gender inequality within the Pamora Group and to analyze the company’s HR data and come up with recommendations for management’s attention.


### DATA SOURCE:
 The primary Data used for this analysis is an Excel Pamora Group HR   Analysis and this Data was gotten from Incubator Hubs.

 
### TOOLS USED
The tools used for this Analysis are:
 - Ms. Power BI
 - Ms. Power Bi  visualization tools

   
### DATA CLEANING AND PRESENTATION
In the initial phase of this process, the Excel Data was loaded into the Power BI and was immediately sent for transformation and inspection. During the transformation process, it was observed that some employees were without Gender, some were without salary because they are no longer with the company while some departments are indicated as “NULL”. A generic Gender was created and other anomalies were remove to make the data 100% accurate for analysis 


### EXPOSITORY DATA ANALYSIS
This involves the exploring of the Data to answer some questions such as:
  - What is the gender distribution in the organization?
  - Show insights on ratings based on gender
  - Analyze the company’s salary structure. Identify if there is a gender pay gap. If there is, identify the department and regions that should be the focus of management
    

### DATA ANALYSIS
The data set was analyzed using some Power BI Measure Slicers and Visualization tools. During the process of the analysis the following  Measures below were used to create addition information for accurate analysis
  - Gender Count = COUNT('Employee'[Gender])`
  - Gender Percentage = DIVIDE(CALCULATE(COUNT('Employee'[Gender])), CALCULATE(COUNT('Employee'[Gender]), ALL('Employee'[Gender])))`
  - `Employees Below Minimum Salary = COUNTX(FILTER('Employee', 'Employee'[Salary] < 90000), 'Employee'[Salary])`
  - Bonus Amount = IF('Employee'[Rating] > 3, 'Employee'[Salary] * 0.1, 0)`
  - - `Total Amount to be Paid = 'Employee'[Salary] + 'Bonus Amount'`

