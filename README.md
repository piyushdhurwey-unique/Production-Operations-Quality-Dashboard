# Production-Operations-Quality-Dashboard

**Tools Used:** Power BI, SQL, DAX, Power Query, Excel  
**Domain:** Manufacturing Operations / Quality Control  

## 📑 Project Overview
In fast-paced manufacturing environments, tracking machine efficiency, net production, and downtime via manual spreadsheets often leads to delayed insights and reactive decision-making. 

This project is an end-to-end Business Intelligence solution designed to monitor daily production metrics and quality control standards. By extracting raw operational data, transforming it via Power Query, and visualizing it in Power BI, this dashboard replaces manual reporting workflows with an automated, real-time analytics pipeline.

## 🎯 Business Problem & Objective
Plant managers need immediate visibility into machine performance and defect rates to meet daily production quotas. The objective of this dashboard is to:
* Automate the calculation of complex manufacturing KPIs.
* Identify the root causes of machine downtime and product defects.
* Provide shift supervisors with actionable insights to optimize resource allocation and improve net production yield.

## 🧰 Tech Stack & Data Pipeline
* **Data Storage / Extraction:** SQL (Simulated relational database containing `Production_Logs`, `Downtime_Records`, and `Quality_Checks` tables).
* **Data Transformation (ETL):** Power Query (Merged tables, handled missing values, standardized shift timestamps).
* **Data Modeling:** Power BI (Built a Star Schema connecting Fact tables to Dimension tables like `Date`, `Machine_ID`, and `Shift_Details`).
* **Calculations:** DAX (Created custom measures for rolling averages, YTD production, and efficiency percentages).
* The data model follows a Star Schema architecture with Machine and Date dimension tables connected to production, downtime, and quality fact tables to ensure       efficient analytics and avoid many-to-many relationships.
