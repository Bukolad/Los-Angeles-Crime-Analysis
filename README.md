# Los-Angeles-Crime-Analysis
This project presents a detailed analysis of crime incidents reported  by the Los Angeles Police Department (LAPD) from 2020 to 2025. The data used for this project was sourced from Data.Gov website with over a million crimes . The goal is to uncover patterns, track crime trends, and provide actionable insights.
# Project Background
Los-Angeles Police Department(LAPD) was established in 1869, LAPD is the primary law enforcement agency serving nearly 4 million residents across 21 areas in Los-Angeles. With a mission to protect and serve, LAPD works to prevent crime, enforce laws, and ensure public safety in one of the most dynamic cities in the world.

From 2020-2025, Los-Angeles recorded hundreds of thousands of crime incidents across its neighbourhood, from downtown LA to Hollywood and South Central. As one of the largest and most diverse cities in the United States, LA's crime patterns reflect complex social dynamics, varying across time, location and severity.
This project presents a comprehensive analysis of over 1 million crime records reported between 2020 and 2025. The aim is to uncover insights into crime trends across different areas, highlight delays in crime reporting, and provide visibility into case outcomes.

# Overview of the Data
The crime dataset used in this project was sourced from Data.Gov website, based on public on public crime records provided by the Los-Angeles Police Department(LAPD). It contained detailed reports of crimes that occured between 2020 and 2025 across various areas of Los-Angeles. The data was cleaned and transformed in Power Query Editor in Power BI
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
- Status : Status of the case.
- Location: Street address of crime incident.
  The CSV file can be downloaded [here](https://catalog.data.gov/dataset/crime-data-from-2020-to-present)
  The major Transformation carried out in Power BI Query Editor include:
  - Removal of Duplicates in the DR-NO
  - Formatting Column by changing the Upper Case to Proper Case.
  - Replacing Values : Values in Victim sex and Victims Descent was changed. Example, F in Victim sex was changed to Female, while H in Victim Descent waas changed to Hispanic/Laotinatian/Mexican.

 # Tools and Technologies used
1. Power BI : This was the major tool used for this project. Power BI was used to create interactive dashboards and visualization for the insights generated from this project.
2. Power Query Editor : The Power Query Editor was used for data cleaning and transformation across different columns such as removing duplicates, replacing values, etc

# Project Workflow
A Project Workflow provides structure for every data analytics project. It helps establish a clear roadmap of sequentials steps, from defining the initial probelm to delivering final insights. This keep the projects organized, aligned with goals, and ensure no critical steps are overlooked.

![image](https://github.com/user-attachments/assets/371ebfb1-59d1-437d-a254-6fee40a9ce65)


# Project Objective
The objectives of this project was to analyze crime trends in Los-Angeles between 2020 and 2025 and provide actionable insights . From this project, it will be easy to understand crime pattern, identify high-crime areas, analyze victim demographics, and tell a data-driven story about the state of crime in Los-Angeles, helping law enforcement agancies, policymakers, and the public make informed decisions.

# Data Collection 
The data for this project was collected from kaggle. The data included crime records from various area in Los-Angeles. 

# Data Cleaning & Preparation
The data cleaning process began in the Power Query Editor in Power BI. The major operation included 
- Removal of duplicates. 
- Text operations such as changing the alphabet case from Upper case to Proper case and replacing values were also carried out on some columns. The M Query [Codes](M.QUERY.txt) from the Power Query Editor have been attached to this repository.
After data cleaning, for easily analysis i added a custom column to group victim's age for easy understanding. In addition, i created new measures and new columns to provide deeper insights into crime trends :
- Average victim age : To profile age trends across crimes.
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
A Calendar Table was created to support year growth comparisons.

# Data Model
The Data Model was automatically created in Power BI. This shows the relationship between the various table in this project.

![image](https://github.com/user-attachments/assets/eb533191-9a3d-4521-b7c8-5d69c426ef2e)


# Data Analysis & Visualization 
After the completion of data cleaning and preparation, i proceeded to begin my analysis and visualization. To ensure easy readability and understanding,i divided the visualization into 5 dashboards. These dashboards were used to effectively visualize key insights from this analysis.

Some key insights from the data visualization are summarized below:
  - ## Overview
 The overview section shows that a total of 1.01 million crimes were recorded in Los-Angeles between 2020 and 2025. However, crime incidents have seen a sharp decline in recent years, with a significant drop of -45% in crime.
  The year 2022 recorded the highest crime volume at 235,000 incidents, making it the peak year in this period. The average age of crime victims is 29 years, with a significant portion falling within the young adult age range. In terms of gender, Male victims accounted for 40.18% while Female victims represented 35.67% and Unknown cases made up 24.14% of the reports.
  When analyzing weapons used, Unspecified methods were the most common, contributing to over 678k incidents, followed by Strong-Arm attacks(hands,fist,bodily force) at 175k cases. Other top weapons included unknown weapons, verbal threats,and handguns.
  The yearly crime trends shows an initial rise from 2020 to 2022, followed by a steep decline in 2024 and 2025. 

![image](https://github.com/user-attachments/assets/a19bb926-5e17-448f-ab8f-9c2aa3b4cca7)


  - ## Time Trends
  The Time Trends analysis shows distinct patterns in criminal activity across different time frames. Crime tend to peak during afternnon and early evening hours, with the 3:00PM TO 5:59PM window showing the highest activity, closely followed by 6:00PM TO 8:59PM. In Contrast, the quietest period occurs between 3:00 AM and 5:59 AM when criminal incidents are at their lowest.
  Monthly patterns show January experiencing the most significant spike in crimes with an 18.6% increase, while also sees a noticeable 3.8% uptick. The months of February,April, June, and September demonstrate declines of -6.8%,-4.9%, -2.0%, -3.4% and -6.1% respectively. Throughout the year, monthly crime counts flunctuate between 78,000 and 93,000 incidents.
  When examining weekly trends, Friday emerges as the peak day for criminal activity approximately 153,700 incidents, followed closely by Saturday with around 147,500 cases. Tuesday consistently shows the lowest crime numbers at about 138,200 reported incidents.
  The Yearly Overview from 2020 to 2025 reveals significant fluctuations. The year 2022 saw the highest volume at 235,000 crimes, followed closely by 2023 with 232,000 crimes with a decline of -2908 crimes. After a modest increase in of 25,000 crimes in 2022, another substantial decline occured in 2023 with over 104,000 fewer crimes.

  ![image](https://github.com/user-attachments/assets/a1b17e12-4662-44bc-bd09-91ca2135266a)

- ## Victim's Demographics
The victim demographics analysis shows that male victims are the most affected group, accounting for 40.18% of reported crimes in Los Angeles between 2020 and 2025. Female victims make up 35.67% of cases, while incidents where the victim’s gender was not recorded account for 24.14%.

When looking at age groups, individuals aged between 35 and 60 years emerged as the most affected, with 327,000 victims reported in this category. This is followed closely by the 0-17 years group, which recorded 295,000 victims, highlighting that both working-age adults and minors are frequently impacted by crime. Cases with unknown victim age were the least represented.

In terms of victim descent, Hispanic, Latino, or Mexican individuals were the most affected, with 296,000 victims recorded. This group was followed by cases where descent was unknown, accounting for 251,000 victims. Other groups included White victims with 201,000 cases, Black victims with 136,000 cases, and individuals categorized under Other descent with 78,000 cases.

This pattern suggests an opportunity to develop targeted victim support and prevention programs, particularly focused on working-age adults and youth, who appear to be most at risk.

![image](https://github.com/user-attachments/assets/b514973d-c70c-4405-bcf6-2e56881087d7)


- ## Crime
The crime analysis for Los Angeles from 2020 to 2025 reveals that vehicle theft was the most frequently committed crime, with 115,000 cases reported. This was followed by simple assault, which recorded 75,000 incidents during the same period.

When examining the types of weapons used in crimes, unspecified weapons accounted for the highest number, with 678,000 cases. Strong-arm tactics, which include the use of hands, fists, and bodily force, were the second most common, with 175,000 incidents. Other notable weapons involved in crimes included other weapons (36,000 cases), verbal threats (24,000 cases), and handguns (20,000 cases).

The data also shows that a total of 21 areas in Los Angeles were covered in this project. The Central Area recorded the highest crime count with 70,000 incidents, while other high-crime areas such as 77th Street, Pacific, and Southwest collectively accounted for 170,000 cases. In contrast, the Foothill Area reported the lowest crime count, with 33,000 incidents.

In terms of crime locations, streets were identified as the top crime premises, with 261,000 cases. This was followed by single-family dwellings, which recorded 164,000 incidents, multi-unit dwellings with 119,000 cases, parking lots with 69,000, and other business locations with 48,000 cases.

![image](https://github.com/user-attachments/assets/ccce571e-73a2-4443-aafd-51258ad2f5c9)


- ## Crimes Report
The crime report analysis reveals that the majority of crimes in Los Angeles were reported early, with approximately 769,000 cases recorded within just two days of the incident. However, there were still noticeable delays in reporting, as about 104,000 cases were reported within one week, 73,000 within one month, and 43,000 within six months. A smaller, yet significant portion around 16,000 cases were reported over six months later, indicating potential barriers or delays in crime reporting among certain cases.

When examining the status of these crimes, it is evident that a large case remains unresolved. Over 804,000 cases are currently marked as Investigation Continuing, reflecting the high volume of ongoing cases within LAPD’s records. Other statuses show 109,000 cases categorized as Adult Other, while 87,000 cases resulted in Adult Arrests. Juvenile-related statuses are lower in volume, with 3,000 cases leading to Juvenile Arrests and 2,000 cases listed as Juvenile Other. A small count of 7 cases remain under unknown status.

This presents an opportunity for the Los Angeles Police Department to strengthen its crime reporting systems, encouraging more timely reports and addressing the underlying causes of delayed reporting.

![image](https://github.com/user-attachments/assets/89656fd0-c2a2-4982-992d-6af1c9d9cc24)


# Conclusion
The analysis of crime data in Los Angeles from 2020 to 2025 reveals important patterns in both crime trends and victim profiles. A total of 1.01 million crimes were reported during this period, with incidents peaking in 2022 before showing a sharp decline in the following years. Vehicle theft and simple assault emerged as the most common crimes, while streets and residential dwellings were identified as the primary locations where these crimes took place.

Victim demographics indicate that males and individuals aged between 35 and 60 years were most frequently affected, while Hispanic and Latino communities reported the highest victim counts. Additionally, the analysis shows that most crimes were reported early, within two days of occurrence, but a significant portion still experienced reporting delays. Over 800,000 cases remain under investigation, reflecting the scale of ongoing efforts required by law enforcement agencies.

Overall, the data highlights both the progress made in reducing crime rates in recent years and the areas that still require focused attention. It provides valuable insights for law enforcement, policymakers, and community leaders seeking to further enhance public safety in Los Angeles.

# Recommendation
- ## Adopt Focused Deterrence Strategies
Los Angeles should implement a focused deterrence model like Group Violence Intervention (GVI), which targets high-risk individuals with a mix of enforcement and community support. Cities like Boston reduced youth homicides by 63% using this strategy. By applying GVI in high-crime areas, LA could achieve up to a 20% reduction in violent crime within 12 months.

- ## Expand Community-Based Violence Intervention (CVI)

Programs like Cure Violence, which treat violence as a public health issue, have reduced shootings by up to 56% in cities like Baltimore and Chicago. LA should train community “violence interrupters” to mediate conflicts early. With strong community engagement, this strategy could cut gun-related incidents by 30% in 18 months.

- ## Use Data-Driven & Predictive Policing

LA can improve crime prevention by using predictive analytics and real-time monitoring to allocate resources where crime is most likely. In cities like Seattle, these systems have led to quicker response times and higher clearance rates. With similar tools, LA could boost clearance rates by 15% and reduce response times by 10% within a year.

- ## Create Trauma Recovery Centers (TRCs)

TRCs offer mental health care, legal help, and counseling for victims of violence. States like Illinois and Ohio have used TRCs to reduce repeat victimization and improve recovery outcomes. Establishing these in LA could reduce repeat incidents by 25% and significantly improve support for victims.

- ## Build Youth Safe Havens & Police Ministations

Creating safe spaces for youth after school with mentorship, recreation, and community policing can lower crime. Boston’s Safe Haven model reduced juvenile crime by 22–27%. If implemented in LA’s high-risk neighborhoods, this could lead to a 30% reduction in youth crime over two years.

- ## Launch Anonymous Reporting Systems in Schools

The “Say Something” program has helped prevent school shootings and resulted in 1,000+ mental health interventions. By adopting this system in LA schools and training students to report warning signs, the city can reduce school violence by 20% over the next three years.

- ## Reform Juvenile Justice with Rehabilitation Focus

Shifting LA’s juvenile justice system toward education, therapy, and skill-building as done in Harris County, Texas can lower reoffending rates. Their Opportunity Center led to a 35% drop in youth recidivism. A similar program in LA could transform outcomes for young offenders.

- ## Enforce Stronger Gun Safety Measures

States like Massachusetts and New York, with strict gun laws, have the lowest firearm death rates nationally. LA can follow their lead by enforcing background checks, red flag laws, and safe storage education. These steps could reduce gun-related crimes by 15% within 18 months.

- ## Streamline Case Investigations and Reduce Backlog
With over 800,000 cases still under investigation, there is an opportunity to improve case resolution processes. Streamlining investigation workflows and increasing resources dedicated to case closures can help reduce the backlog and deliver quicker justice outcomes.

- ## Encourage Timely Crime Reporting and Address Delays
Efforts should be made to enhance crime reporting mechanisms to ensure incidents are reported promptly. Special attention should be given to addressing cases that are currently delayed by several months, through community education and by removing barriers that prevent timely reporting.
