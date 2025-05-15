# HEALTH CARE DASHBOARD REPORT

### Introduction
This dashboard provides a comprehensive view of key health indicators, patients metrics, operational performance and clinical outcomes. It consolidates complex health care data into interactive dynamic charts, graphs, and KPIs to support real-time monitoring, decision-making and strategic planning.

### Executive Summary
This report provides an in-depth analysis of patient demographics, medical conditions, test results, hospital performance, and billing insights, based on aggregated data from a healthcare system spanning multiple facilities and admission types. The data is visualized across three comprehensive dashboards—Patient Overview, Billing Summary, and Hospitals & Test Results—providing stakeholders with a clear understanding of healthcare trends, operational efficiency, and financial performance.

###bData Sources
- [Download Here](https://drive.google.com/file/d/11AG3jVY8n0Rm4E53ty36TuNfzz4QHADI/view?usp=drivesdk)

### Tools Used
- Microsoft Excel for Data Cleaning.
- Microsoft Excel for Data Visualization.

### Data Cleaning and Data Preparation
- Over 55,000 records from the year 2019-2024
- Removal of duplicates.
- Standardizing text columns.
- Ensuring each column are in the right and appropriate formats e.g. Date, numbers, text, currency.
- Created a new column named ‘Length of Stay’ (LOS) for each patient. This was achieved by getting the date difference between ‘Date of Discharged’ column and the ‘Date of Admission’ column and making the exact day of admission inclusive.
- Created a new column named ‘Daily Cost’ for each patient. This was achieved by dividing the total billing amount for each patient by their length of stay.

### Data Modelling
After ensuring my data’s accuracy and consistency, I began the process of creating a data model for my table by structuring the dataset to 8 different tables. I first establish my data table which is “Fact table” then started creating relationships between tables. For this project, I used “one to many” relationship. Screenshot of the completed model is attached below.


### DAX Function 
With the table relationships established, I utilized some DAX functions to analyze the dataset. I started by creating basic KPIs such Total Billing Amount, Average Billing Amount, Number of Patients, Hospitals, etc. This would help in creating more advanced metrics later on. 

![Excel Model](https://github.com/user-attachments/assets/d39927de-036d-41fc-945e-dfafbcb19945)

![Excel Dax](https://github.com/user-attachments/assets/fb8b2f7a-6235-4ca9-9700-35783f3210a2)


### Dashboard Structure and Visual Highlights
**Patients Overview Dashboard**

**Key Metrics**


- Total Patients: 54,943
- Emergency Admission Ratio: 32.3%
- Average Age: 52 years
- Average Length of Stay (LOS): 15.52 days
- Gender Distribution: Male – 50.02%, Female – 49.98%
  
**Admissions Trend**


Patient admissions display a clear seasonal pattern, with noticeable peaks mid-year (June–August), suggesting higher healthcare demand during those months.


**Age Group Analysis**


Patients predominantly fall within the 53–62 age bracket, followed by 43–52 and 63–72. This indicates a high utilization of healthcare services by older adults.


**Medical Condition Breakdown**


Top conditions include Hypertension, Diabetes, Cancer, and Asthma. Elective admissions dominate chronic conditions like diabetes and hypertension.


**Medication Distribution**


Prescribed drugs are Aspirin, Ibuprofen, Lipitor, Paracetamol, and Penicillin. Aspirin and Paracetamol dominate elective admissions.

**Blood Type & Gender Distribution**


Common blood types are B+ and O+. Gender distribution is nearly equal across all blood types.

**Test Results**


- Normal Results: 33.35%


- Abnormal Results: 33.54%


- Inconclusive Results: 33.11%

![1](https://github.com/user-attachments/assets/29f2b8c2-e6ff-489a-992e-312ed3945568)

**Hospitals & Test Results Dashboard**


**Hospital Statistics**


- Total Hospitals: 39,880

  
- Total Doctors: 40,340

**Test Result Trends**


- Abnormal: 33.47%
- Normal: 33.48%
- Inconclusive: 33.04%

**Medical Conditions & Test Outcomes**


Conditions like Asthma, Cancer, Diabetes, and Hypertension show balanced test result distributions.

**Admission Type vs Test Results**


Elective admissions show higher test activity. Emergency cases lead to more abnormal or inconclusive results.

**Top 5 Hospitals with Doctors and their Daily Cost Analysis**


Most Doctors: Topped by LLC Smith Hospital with 40 Doctors, while Highest Daily Cost: Johnson Plc, followed by Smith Ltd Hospital.

**Top 5 Hospital Capacity** 


Most Room Capacity: LLC Smith with 38 rooms, while Smith Group 31 rooms.


**Hospital Admission Mix**


Hospitals generally show an even mix of admission types, with some specializing in elective procedures.

![2](https://github.com/user-attachments/assets/1ed687a2-7315-4ea6-9895-a265998a5159)


**Billing Summary Dashboard**


**Key Metrics**

- Total Billing Amount: $1.40 Billion
- Average Billing per Patient: $25,545
- Emergency Billing Total: $461.70 Million
- Average Daily Cost per Patient: $3,390


**Billing by Month**


Billing peaks align with mid-year increases in patient admissions, especially from May through August.



**Billing by Medical Condition**


Highest costs are seen in Obesity, Diabetes, Arthritis and Hypertension,  some of which require longer stays and more medication.

**Billing by Medication**


Ibuprofen and Paracetamol contribute significantly to total costs. Aspirin remains low-cost yet widely used.

**Gender-Based Billing Contribution**


Male Patients: 50.16%, Female Patients: 49.84%. This reflects equitable access and cost-sharing across genders.

**Insurance Providers Analysis**


Highest Average Billing: Medicare and Blue Cross. Lowest: UnitedHealthcare. Policy differences likely affect this trend.

**Correlation Analysis**


- Age vs Billing Amount: Weak positive correlation (R² = 0.004)


- LOS vs Billing Amount: Weak negative correlation (R² = 0.0096)


![3](https://github.com/user-attachments/assets/a2147e8d-2446-48ab-a0a1-f4f751608f7e)


### Conclusion
- Seasonal trends influence both admissions and billing.
- Chronic diseases drive healthcare costs.
- Weak correlation exists between age/LOS and billing.
- Balanced test results suggest standardized procedures.


### Recommendations
- Target preventive care programs for older adults.
- Optimize medication costs through procurement policies.
- Audit high-cost hospitals for efficiency.
- Improve diagnostic accuracy to reduce inconclusive results



