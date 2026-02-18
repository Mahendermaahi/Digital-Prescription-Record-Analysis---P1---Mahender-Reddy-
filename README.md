# Digital-Prescription-Record-Analysis



**Project Overview:** 



This project focuses on digital prescription data management and analysis in the healthcare domain. It helps in managing, tracking, and analyzing electronic medical prescriptions to improve:



&nbsp; 1)Record keeping



&nbsp; 2)Patient safety



&nbsp; 3)Process efficiency for healthcare providers



The system uses a Python-based ETL pipeline and MySQL database to clean, validate, and analyze prescription data.



**Objective:**



Digitize prescription management to reduce errors



Enable real-time tracking and secure record storage



Analyze prescription data for trends and quality monitoring



**Business Rules to Be Implemented:**



Age must be between 0–100



Duplicate prescriptions are invalid



Prescriptions without valid patient/doctor are rejected



Missing dosage/frequency → "Not Provided"



Unknown gender → "U"



**Business Insights to be implemented using matplotlib:**



Most frequently prescribed medicines

Doctor-wise prescription volume comparison

Gender-wise prescription distribution

Age group vs number of prescriptions

Detect doctors issuing unusually high prescriptions

Daily prescription trend over time

Data quality comparison (before vs after cleaning)



**ETL Pipeline Flow:**



CSV files (dirty data)

&nbsp;       ↓

Python ETL (Pandas)

&nbsp; - Deduplication

&nbsp; - Null handling

&nbsp; - Business rules

&nbsp;       ↓

MySQL clean tables (DDL + constraints)

&nbsp;       ↓

SQL analytics + Matplotlib dashboards





**Technologies Used:** 



Python

Pandas

numpy

MySQL

Matplotlib

SQL



**ETL Pipeline (Step-by-Step Process):**



**Step 1: Data Collection**



Raw CSV files with dirty/incomplete data are collected.



**Step 2: Data Cleaning**



Using Pandas:



Remove duplicates



Handle null values



Apply business rules



Standardize data formats



**Step 3: Apply Business Rules**



Age must be between 0–100



Duplicate prescriptions are invalid



Prescriptions without valid patient/doctor are rejected



Missing dosage/frequency → "Not Provided"



Unknown gender → "U" 



6fdfea99-e578-4661-87b6-631cca8…



**Step 4: Data Storage**



Cleaned data is stored in MySQL tables with:



DDL



Constraints



Proper relationships



**Step 5: Data Analysis**



SQL queries are used to analyze trends.



**Step 6: Visualization**



Matplotlib dashboards are created to visualize insights.



ETL Flow:

CSV → Python Cleaning → MySQL → SQL Analysis → Visualization



**Business Insights Generated:** 



Most frequently prescribed medicines



Doctor-wise prescription comparison



Gender-wise prescription distribution



Age group vs prescription count



Detect unusually high prescriptions by doctors



Daily prescription trends



Data quality comparison (before vs after cleaning)







