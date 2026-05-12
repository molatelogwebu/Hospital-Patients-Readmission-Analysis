Hospital Readmission Analysis

- Analysing hospital readmission trends using Excel.

Project Overview

This project analyzes hospital readmission data to identify patterns and factors contributing to patient readmissions.

Dataset description:

Source: Kaggle - hospital patient readmission dataset

Records: (8000 patient records) 

Key Features:

- Patient demographics (age, gender)

- Medical conditions / diagnoses

- Number of prior visits

- Length of stay

- Medications and treatments

Target Variable:

- Readmission Status 


Objectives

- Identify key factors influencing readmissions
- Analyze trends across patient groups
- Support healthcare decision-making

Key Insights

- For some patients, the rate of readmission is high
  
- Patients who stay long at hospitals have high chances of readmission
  
- There are some conditions that are related to readmission
  
- Intervening early helps in reducing readmission

Business Recommendations:

Considering the analysis conducted on the readmissions rate among patients at hospitals, the following business recommendations can assist healthcare providers to achieve better results:

- Create a follow-up program for patients who are considered at high risk of being readmitted

- Enhance the discharge process and educate patients to prevent unnecessary readmissions

- Utilize advanced analytics to recognize patients with higher chances of being readmitted

- Assign additional funding to departments with high readmission rates

- Offer more preventive care services for chronic diseases management

- Create interactive dashboards to track key indicators of readmission and hospital performance

  
Tools Used
- Excel
- Power Bi

Methodology:

- Data Cleaning:  
1. Checked for duplicates — none found.
2. Handled missing values:
a.  Text Columns:
=IF(C2="";”UNKNOWN”C2)

b. Numeric Columns:
=IF(B2="";0; H2)

c. Standardized text columns using:
=PROPER(TRIM(F2))
=UPPER(TRIM(E2))

d.  Validate Age:
=IF(OR(D2<0;D2>120),”CHECK”D2)

Calculations;
1. Age Group
=IF(D2<18;”Child”;IF(D2<40;”Young Adult; IF(D2<65;”Adult”, “Senior”)))

2. Admission Month
= TEXT(B2;”MMM”)

3. Admission Year
= YEAR(B2)

4. Readmission Risk Category
=IF(P2<0.3,"Low",
IF(P2<0.7,"Medium","High"))

5. Frequent Patient Flag
=IF(M2>=3,"Frequent","Normal")

Link to PowerBI; 
https://app.powerbi.com/groups/me/reports/5c89e5c2-dfc5-411c-9819-b371667ee48a/669cb6ba0ac9040b050d?experience=power-bi

Dataset source:
Kaggle.com 

Author
- Molatelo Gwebu
