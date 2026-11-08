# 🏥 Hospital Management System – SQL & Power BI Analytics

![MySQL](https://img.shields.io/badge/Database-MySQL-blue?logo=mysql)
![Power BI](https://img.shields.io/badge/Visualization-Power%20BI-yellow?logo=powerbi)
![SQL](https://img.shields.io/badge/Language-SQL-orange)
![Project](https://img.shields.io/badge/Project-Data%20Analytics-teal)

## 📌 Project Overview

The **Hospital Management System – SQL & Power BI Analytics** project focuses on analysing hospital operations, patient behaviour, doctor performance, appointment management and treatment revenue.

The project uses **MySQL** for database management and SQL-based analysis, and **Microsoft Power BI** for interactive dashboard development and business intelligence reporting.

The objective is to transform raw hospital data into meaningful insights that can help hospital management monitor operational performance and make data-driven decisions.

## 🎯 Business Problem

Hospitals generate large amounts of operational data related to patients, doctors, departments, appointments, treatment costs and payment methods.

However, without proper analysis, management may find it difficult to:

- Monitor appointment completion and cancellation rates.
- Understand patient registration and visit patterns.
- Evaluate doctor and department performance.
- Identify high-revenue departments.
- Analyse treatment costs and payment methods.
- Monitor patient satisfaction through ratings.
- Identify repeat patients and patient retention patterns.

This project addresses these challenges through SQL analysis and interactive Power BI dashboards.

## 🎯 Project Objectives

1. Design and implement a relational database using MySQL.
2. Perform data exploration and analysis using SQL.
3. Answer 38 business questions using SQL queries.
4. Analyse hospital revenue, appointments and operational KPIs.
5. Evaluate doctor and department performance.
6. Understand patient demographics and repeat visits.
7. Develop interactive dashboards using Power BI.
8. Present actionable business recommendations based on analytical findings.

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| MySQL | Database management |
| MySQL Workbench | SQL development and query execution |
| SQL | Data extraction, transformation and analysis |
| Microsoft Power BI | Interactive dashboard development |
| DAX | KPI calculations and measures |
| Power Query | Data transformation and preparation |
| GitHub | Project documentation and version control |
| PowerPoint | Project presentation |

## 📂 Dataset Overview

The project uses a fictional hospital management dataset containing 4 relational tables and 98 records.

| Table | Records | Description |
|---|---:|---|
| Departments | 8 | Department details and floor numbers |
| Doctors | 10 | Doctor information, experience and consultation fees |
| Patients | 30 | Patient demographics and registration details |
| Appointments | 50 | Appointment details, treatment costs, payment modes, status and ratings |
| **Total** | **98** | **Complete dataset** |

### Database Schema

The database is named `HospitalDB`.

**Tables and relationships:**

- Departments → Doctors (One-to-Many)
- Doctors → Appointments (One-to-Many)
- Patients → Appointments (One-to-Many)

The `Appointments` table connects the patient and doctor records using foreign keys.

### Database Relationship Diagram

Add your database schema screenshot here:

`![Database Schema](Dashboard_Screenshots/database_schema.png)`

## 📊 SQL Analysis

A total of **38 business questions** were explored using SQL to understand different aspects of hospital operations.

### SQL Concepts Covered

**1. Basic SQL Operations**
- SELECT and DISTINCT
- WHERE
- BETWEEN
- IN
- IS NULL
- ORDER BY
- LIMIT

**2. Aggregate Functions**
- COUNT()
- SUM()
- AVG()
- MIN()
- MAX()

**3. Grouping and Filtering**
- GROUP BY
- HAVING

**4. Joins**
- INNER JOIN
- LEFT JOIN
- Multi-table joins

**5. Subqueries**
- Single-row subqueries
- Multiple-row subqueries
- Nested queries
- EXISTS and NOT EXISTS

**6. Advanced SQL**
- Common Table Expressions (CTEs)
- Window Functions
- DENSE_RANK()
- LAG()

### Business Questions Explored

The SQL analysis covers:

- Patient and doctor information.
- Appointment status and completion rate.
- Department-wise revenue.
- Doctor-wise revenue.
- Average patient ratings.
- City-wise patient distribution.
- Most common diseases.
- Payment-mode analysis.
- Repeat patient identification.
- Top-performing doctors.
- Revenue ranking within departments.
- Previous appointment cost analysis.

### SQL Query Screenshots

Add your SQL query screenshots in the `SQL_Screenshots` folder.

Example:

| Analysis | Screenshot |
|---|---|
| Data Exploration | `01_data_exploration.png` |
| Aggregate Analysis | `02_aggregate_analysis.png` |
| Join Analysis | `03_joins_analysis.png` |
| Subqueries | `04_subqueries.png` |
| CTE Analysis | `05_cte_analysis.png` |
| Window Functions | `06_window_functions.png` |

## 📈 Power BI Dashboard

The project includes three interactive Power BI dashboard pages developed using data connected from MySQL.

### 1. Hospital Performance Overview

This dashboard provides an overview of hospital operations and financial performance.

Key metrics:
- Total Doctors: 10
- Total Patients: 30
- Total Appointments: 50
- Completed Appointments: 48
- Pending Appointments: 1
- Cancelled Appointments: 1
- Completed Treatment Revenue: ₹182,200

Visualizations:
- Appointment status distribution.
- Department-wise revenue.
- Appointment trends over time.
- Date and department filters.

![Hospital Performance Overview](Dashboard_Screenshots/dashboard_overview.png)

### 2. Doctor & Department Analysis

This dashboard focuses on doctor productivity and department performance.

Key metrics:
- Total Doctors: 10
- Total Departments: 8
- Average Patient Rating: 4.44
- Average Consultation Fee: ₹985
- Completed Treatment Revenue: ₹182.2K

Visualizations:
- Doctor-wise revenue comparison.
- Department-wise appointment distribution.
- Average rating by doctor.
- Doctor and department filters.

![Doctor and Department Analysis](Dashboard_Screenshots/doctor_department_analysis.png)

### 3. Patient & Appointment Analysis

This dashboard provides insights into patient demographics, diseases and appointment behaviour.

Key metrics:
- Total Patients: 30
- Total Appointments: 50
- Appointment Completion Rate: 96%
- Repeat Patients: 18

Visualizations:
- City-wise patient distribution.
- Disease distribution.
- Gender distribution.
- Appointment status analysis.
- Doctor and date filters.

![Patient and Appointment Analysis](Dashboard_Screenshots/patient_appointment_analysis.png)

## 🔍 Key Insights & Findings

The analysis revealed the following findings:

### Hospital Performance

- The hospital recorded 50 appointments.
- 48 appointments were completed.
- The appointment completion rate was 96%.
- There was 1 pending appointment and 1 cancelled appointment.
- Completed treatment revenue was ₹182,200.

### Department Performance

| Department | Completed Revenue |
|---|---:|
| Cardiology | ₹62,200 |
| Orthopedics | ₹37,600 |
| Gynecology | ₹22,100 |
| Neurology | ₹18,900 |
| General Medicine | ₹14,900 |
| Dermatology | ₹13,800 |
| Pediatrics | ₹7,700 |
| ENT | ₹5,000 |

**Key finding:** Cardiology generated the highest completed treatment revenue of ₹62,200.

### Doctor Performance

- Dr. Amit Sharma generated the highest completed treatment revenue of ₹62,200.
- Dr. Pooja Nair recorded the highest average patient rating of 5.00.
- Cardiology recorded the highest appointment count, with 9 appointments.

### Patient Analysis

- 30 patients were recorded in the database.
- The patient population consisted of 15 male and 15 female patients.
- 18 patients had at least two completed appointments.
- Hyderabad recorded the highest patient count, with 6 patients.

### Payment Analysis

Insurance contributed ₹100,000 towards completed treatment revenue, making it the highest-revenue payment mode.

## 💡 Business Recommendations

Based on the findings, the following recommendations can be considered:

1. **Appointment Monitoring:** Continue monitoring pending and cancelled appointments to maintain a high completion rate.
2. **Department Performance:** Study the factors contributing to higher revenue and appointment volumes in Cardiology and Orthopedics.
3. **Doctor Performance:** Evaluate doctors using a combination of workload, completed revenue and patient ratings.
4. **Patient Retention:** Analyse repeat patient behaviour to understand recurring visits and improve patient engagement.
5. **Payment Analysis:** Monitor payment-mode contribution, particularly insurance payments.
6. **Patient Satisfaction:** Regularly review patient ratings and feedback to identify opportunities for service improvement.

## 📁 Project Structure

The GitHub repository is organized as follows:

```text
Hospital-Management-Analytics/
│
├── README.md
│
├── Database/
│   └── Hospital_Database.sql
│
├── SQL_Analysis/
│   └── Hospital_Queries.sql
│
├── PowerBI/
│   └── Hospital_Management_Dashboard.pbix
│
├── Reports/
│   ├── Business_Requirements_Document.pdf
│   └── Hospital_Management_Analytics_Presentation.pptx
│
├── SQL_Screenshots/
│   ├── 01_data_exploration.png
│   ├── 02_aggregate_analysis.png
│   ├── 03_joins_analysis.png
│   ├── 04_subqueries.png
│   ├── 05_cte_analysis.png
│   └── 06_window_functions.png
│
└── Dashboard_Screenshots/
    ├── database_schema.png
    ├── dashboard_overview.png
    ├── doctor_department_analysis.png
    └── patient_appointment_analysis.png
```

## ⚙️ How to Run This Project

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/Hospital-Management-Analytics.git
```

### Step 2: Open MySQL Workbench

- Open MySQL Workbench.
- Connect to your MySQL Server.
- Open `Database/Hospital_Database.sql`.
- Execute the complete SQL script.
- Verify that the `HospitalDB` database and all four tables have been created.

### Step 3: Execute SQL Queries

- Open `SQL_Analysis/Hospital_Queries.sql`.
- Select the required query.
- Execute it using the lightning-bolt button.
- Review the output in the result grid.

### Step 4: Open Power BI Dashboard

- Open Microsoft Power BI Desktop.
- Install the required MySQL Connector/NET driver if needed.
- Connect to the `HospitalDB` database.
- Load the Departments, Doctors, Patients and Appointments tables.
- Recreate the data model and measures if necessary.
- Open the supplied `.pbix` file.

**Note:** If the PBIX file uses a local MySQL connection, update the server credentials and connection settings before refreshing the data.

### Step 5: Explore the Dashboards

Use the date slicers, doctor filters and department filters to interact with the three dashboard pages.

## 📌 Key Performance Indicator Definitions

| KPI | Calculation |
|---|---|
| Total Patients | Distinct count of patient IDs |
| Total Doctors | Distinct count of doctor IDs |
| Total Appointments | Count of appointment records |
| Completed Appointments | Count where status = Completed |
| Completed Treatment Revenue | Sum of treatment cost for Completed appointments |
| Completion Rate | Completed Appointments / Total Appointments × 100 |
| Average Rating | Average of completed appointment ratings |
| Repeat Patients | Patients with at least two completed appointments |

**Important:** Pending and cancelled appointments are excluded from completed treatment revenue. NULL ratings are not treated as zero.

## ⚠️ Assumptions & Limitations

- All records are fictional and created for learning and portfolio demonstration.
- The dataset contains 98 records and is relatively small.
- Treatment cost is treated as recorded completed appointment revenue.
- The project does not model refunds, insurance settlements, outstanding balances or operating expenses.
- Revenue should not be interpreted as hospital profit.
- Patient ratings are nullable and only available for rated appointments.
- The analysis is intended for business analytics demonstration, not clinical decision-making.

## 🚀 Skills Demonstrated

- Relational Database Design
- MySQL Database Management
- SQL Query Writing
- Data Exploration
- Data Aggregation
- Joins and Subqueries
- CTEs and Window Functions
- Business KPI Analysis
- Data Modelling
- DAX Measures
- Power Query
- Power BI Dashboard Development
- Business Insights and Recommendations
- Data Storytelling

## 👨‍💻 Author

**SK Abdul Samad**

Data Analyst | SQL | Power BI | Python | Data Analytics

- GitHub: [Your GitHub Profile](https://github.com/your-username)
- LinkedIn: [Your LinkedIn Profile](https://www.linkedin.com/in/your-profile/)

---

Hospital-Management-Analytics/
│
├── README.md
├── Database/
│   └── Hospital_Database.sql
├── SQL_Analysis/
│   └── Hospital_Queries.sql
├── PowerBI/
│   └── Hospital_Management_Dashboard.pbix
├── Reports/
│   ├── Business_Requirements_Document.pdf
│   └── Project_Presentation.pptx
├── SQL_Screenshots/
└── Dashboard_Screenshots/

**Project Takeaway**

"Transforming relational hospital data into meaningful business insights through SQL analysis and interactive Power BI dashboards."

*This project uses synthetic data and is intended exclusively for educational and portfolio purposes.*
