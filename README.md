# Los-Angeles-Crime-Analysis
This project presents a detailed analysis of crime incidents reported  by the Los Angeles Police Department (LAPD) from 2020 to 2025. The data used for this project was sourced from Kaggle with over a million crimes . The goal is to uncover patterns, track crime trends, and provide actionable insights.
# Project Background
Los-Angeles Police Department(LAPD) was established in 1869, LAPD is the primary law enforcement agency serving nearly 4 million residents across 21 areas in Los-Angeles. With a mission to protect and serve, LAPD works to prevent crime, enforce laws, and ensure public safety in one of the most dynamic cities in the world.

From 2020-2025, Los-Angeles recorded hundreds of thousands of crime incidents across its neighbourhood, from downtown LA to Hollywood and South Central. As one of the largest and most diverse cities in the United States, LA's crime patterns reflect complex social dynamics, varying across time, loaction and severity.
This project presents a comprehensive analysis of over 1 million crime records reported between 2020 and 2025. The aim is to uncover insights into crime trends across different areas, highlight delays in crime reporting, and provide visibility into case outcomes.

# Overview of the Data
The crime dataset used in this project was sourced from Kaggle, based on public on public crime records provided by the Los-Angeles Police Department(LAPD). It contained detailed reports of crimes that occured between 2020 and 2025 across various areas of Los-Angeles. The data was cleaned and transformed in Power Query Editor in Power BI
## Key Data Columns
- DR-NO - Divisions Record Number.
- Date Reported : The date when the crime was officially reported. 
- Date Occured : The actual date when the crime took place.
- Time Occured : The time of day when the crime occured.
- Area Name: Geographic divisions of LAPD.
- Crime : The description of the crime.
- Victim's Age : The age of the victim involved in the crime.
- Victim's Sex : The sex of the victim imvolved in the crime.
- Victim's Descent : The code indicating the victim's ethnicity.
- Premise : Decription of the location type where the crime occured.
- Weapon :  Type of weapon used for the crime.
- Status : Staus of the case.
- Location: Street address of crime incident.
  The CSV file can be downloaded [here](https://catalog.data.gov/dataset/crime-data-from-2020-to-present)

 # Tools and Technologies used
1. Power BI : This was the major tool used for this project. Power BI was used to create interactive dashboards and visualization for the insights generated from this project.
2. Power Query Editor : The Power Query Editor was used for data cleaning and transformation across different columns such as removind duplicates, replacing values, etc

# Project Workflow
A Project Workflow provides structure for every data analytics project. It helps establish a clear roadmap of sequentials steps, from defining the initial probelm to delivering final insights. This keep the projects oragnized, aligned with goals, and ensure no critical steps are overlooked.

# Project Objective
The objectives of this project was to analyze crime trends in Los-Angeles between 2020 and 2025 and provide actionable insights . From this project, it will be easy to understand crime pattern, identify high-crime areas, analyze victim demographics, and tell a data-driven story about the state of crime in Los-Angeles, helping law enforcement agancies, policymakers, and the public make informed decisions.

# Data Collection 
The data for this project was collected from kaggle. The data included crime records from various area in Los-Angeles. 

# Data Cleaning & Preparation
The data cleaning process began in the Power Query Editor in Power BI. The major operation included 
- Removal of duplicates. 
- Text operations such as capitalising each words and replacing values were also carried out on some columns. The M Query Codes from the Power Query Editor have been attached to this repository.
After data cleaning, for easily analysis i added a custom column to group victim's age for easy understanding. In addition, i created new measures and new columns to provide deeper insights into crime trends :
- Average victim age : To profile age trends across crimes
- Blank measure for month and year : to
- Condition formatting growth : This measure was created to highlight month and year growth. if the growth is positive(increase in crime), it shows in red. if negative(crime reduced), it shows in green.
- Crimes last year and this year : This measure was created to compare crime counts across years.
- Max Crime Year : To identify which year recorded the highest crime rate.
- Total Crimes : To calculate the total crimes from 2020-2025.
- Percentage increase in Crime : To calculate the increase in crime each year
- Year Growth : Change in crime volume each year
  
Additonal Transformation included
- Created new Column to calculate Report Days( the difference between Date Reported and Date Occurred)
- New Column was created to group the Report Days for easy analysis
- New Column was creatd to calculate the Time Range and Victim's Age Group.
A Calendar Table was created to support year growth comparisons 
  Click here to view DAX functions used to create the measures, calculated columns and Table.

# Data Model
The Data Model was automatically created in Power BI. This shows the relationship between the various table in this project.

# Data Analysis & Visualization 
After the completion of data cleaning and preparation, i proceeded to begin my analysis and visualization. To ensure easy readability and understanding,i divided the visualization into 5 dashboards. These dashboards were used to effectively visualize key insights from this analysis.

Some key insights from the data visualization are summarized below:
- Overview: This overview section provides the summary of crime statistics in Los-Angeles. Key insights include:
   - The overview section shows the total of 1.01 million crimes committed from 2020-2025
