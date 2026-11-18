# 📊 Digilians Trainees Performance Dashboard (End-to-End SQL & Power BI)

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=for-the-badge&logo=microsoft-sql-server&logoColor=white)
![Data Analysis](https://img.shields.io/badge/Data%20Analysis-0078D4?style=for-the-badge&logo=databricks&logoColor=white)

## 📌 Project Overview
An end-to-end data analytics project designed to monitor, evaluate, and analyze trainees' academic performance and attendance across multiple labs (`LAB5` to `LAB8`) under the **Digital Egypt Pioneers Initiative (Digilians)**. 

The workflow starts with relational database schema creation and data ingestion in **SQL Server**, followed by analytical querying, views creation (`v_SessionAttendance`, `v_TraineePerformance`), DAX calculations, and interactive visualization in **Power BI**.

---

## 🖼️ Dashboard Preview
![Dashboard Preview](Assets/dashboard_preview.png)

---

## 🎯 Key Performance Indicators (KPIs)
* **Total Trainees:** `138` trainees across multiple Egyptian universities and labs.
* **Overall Attendance Rate:** `68.91%`
* **Average Final Score:** `73.33`
* **Fail Rate:** `6.52%`

---

## 💡 Key Analytical Insights
1. **Academic Performance Tiering:** Over **51%** of trainees achieved a `B` grade, while **28.99%** achieved a `C`, and only **6.52%** fell into the failing tier.
2. **University & Gender Distribution:** Mansoura University represents the largest cohort of trainees, followed by Cairo University, Ain Shams University, and Misr International University (MIU).
3. **Session Attendance Trends:** Attendance status (`Present`, `Late`, `Absent`) was tracked across core SQL modules (e.g., `SELECT`, `JOIN`, `GROUP BY`, `CTE`, `Window Functions`, `Subqueries`), highlighting consistent engagement across technical topics.
4. **Instructor Evaluation:** Tracked average trainee scores per instructor to benchmark instructional effectiveness across labs.

---

## 🛠️ Technical Workflow & Repository Structure

### 1. Database Engineering & SQL (`SQL_Scripts/`)
* **`01_Create_Tables.sql`**: Designed normalized database tables with primary/foreign key constraints to store trainees, labs, sessions, attendance, and grades.
* **`02_Load_Data_for_all_LABs.sql`**: Populated and consolidated data across multiple training labs (`LAB5 A-FF-05` through `LAB8 A-GF-13`).
* **`03_Analytical_Questions.sql`**: Answered core business and academic questions using aggregations, joins, and custom SQL views (`v_SessionAttendance`, `v_TraineePerformance`) to feed the reporting layer.

### 2. Data Modeling & Visualization (`Dashboard/`)
* Connected Power BI directly to SQL Server views.
* Built custom **DAX Measures** for `Attendance Rate`, `Fail Rate`, `Average Final Score`, and `Total Trainees`.
* Implemented interactive slicers by **University** and **Lab Code** for dynamic drill-down analysis.

---

## 🚀 How to Reproduce
1. Execute `01_Create_Tables.sql` in **SQL Server Management Studio (SSMS)** to build the database schema.
2. Run `02_Load_Data_for_all_LABs.sql` to insert the lab records.
3. Run `03_Analytical_Questions.sql` to generate the analytical queries and views.
4. Open `Digilians Trainees Performance Dashboard.pbix` in **Power BI Desktop** and refresh the data source connection.

---

## 👤 Author
**Taha Kamel**  
*Data Analyst | Microsoft Certified: Power BI Data Analyst Associate (PL-300)*  
[LinkedIn](https://www.linkedin.com/) | [Portfolio / Linktree](https://linktr.ee/)
