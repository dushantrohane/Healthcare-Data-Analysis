🏥 Healthcare Analytics Dashboard – Power BI

A comprehensive and interactive Power BI dashboard designed to analyze key healthcare performance metrics such as patient flow, treatment success, readmission rate, billing trends, and waiting time. This report helps hospitals and administrators make data-driven decisions to improve patient experience and operational efficiency.

📌 Project Overview
   This Power BI project focuses on visualizing and analyzing hospital operational data. The dashboard provides insights into:

  -Patient demographics
  -Treatment success and failure rates
  -Waiting time and treatment duration
  -Readmission rate
  -Department-wise performance
  -Billing and revenue trends
  -Patient flow patterns over time

🎯 Objectives

  -Identify bottlenecks in patient processing
  -Monitor hospital performance KPIs
  -Improve patient experience by reducing wait times
  -Track financial performance and billing insights
  -Support data-driven decision-making for hospital management

📂 Dataset Description

The dataset includes the following key columns:

  -Patient_ID
  -Name / Gender / Age
  -Department / Doctor_Name
  -Symptoms / Diagnosis / Treatment
  -Treatment_Start / Treatment_End
  -Admission_Date / Discharge_Date
  -Readmission_Flag
  -Billing_Amount

📊 Dashboard Insights
✔️ 1. Patient Overview

  Total patients
  Gender ratio
  Age distribution
  Department-wise count

✔️ 2. Treatment Analysis

  Treatment success rate
  Failure or incomplete cases
  Average treatment duration

✔️ 3. Waiting Time

  Average waiting time per department
  Longest & shortest wait times

✔️ 4. Readmission Rate

  Formula used:
  Readmission Rate = (Number of patients marked as Readmitted) / (Total Patients)

✔️ 5. Revenue Dashboard

  Total Billing Amount
  Department-wise Revenue
  Billing trend over time

✔️ 6. Patient Flow

  Daily / weekly / monthly patient volume
  Peak hours / peak days

🧮 Important DAX Measures Used
Waiting Time
Waiting Time (Minutes) =
DATEDIFF([Admission_Date], [Treatment_Start], MINUTE)

Treatment Duration
Treatment Duration (Minutes) =
DATEDIFF([Treatment_Start], [Treatment_End], MINUTE)

Treatment Success Rate
Success Rate =
DIVIDE(COUNTROWS(FILTER('Table', 'Table'[Treatment_Status] = "Success")),
COUNTROWS('Table'))

Readmission Rate
Readmission Rate =
DIVIDE(COUNTROWS(FILTER('Table', 'Table'[Readmission_Flag] = "Yes")),
COUNTROWS('Table'))

🛠️ Tools & Technologies Used

  -Power BI Desktop
  -Power Query for data transformation
  - DAX for calculated columns & measures
  -Data Modeling (Star Schema)
  -Interactive Visualizations & KPIs

📥 How to Use the File

-Download the .pbix file from this repository
-Open it with Power BI Desktop
-Refresh the data source if needed
-Explore and customize the dashboard

🚀 Future Improvements

-Integrate real-time hospital data using APIs
-Add predictive modeling for readmission risk
-Create automated alerts for high waiting times
-Develop a Power BI Service dashboard for live monitoring

🤝 Contributions

Contributions are welcome!
Feel free to report issues, suggest improvements, or submit pull requests.

📧 Contact

Dushant Rohane
Data Analyst

Email: dushantrohane@gmail.com

GitHub: github.com/dushantrohane

LinkedIn: linkedin.com/in/dushant-rohane/
