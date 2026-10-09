# 📊 Ticket Performance & Working Time Analysis

An interactive Power BI dashboard designed to analyze ticket performance, working time, operational efficiency, and employee productivity. The project uses DAX measures and interactive visualizations to evaluate ticket resolution performance across management, activity, and employee perspectives.

## Project Overview

This project focuses on analyzing operational ticket data to understand workload distribution, resolution performance, working time, and employee productivity.

The dashboard provides insights into ticket volumes, success and failure rates, activity categories, departments, processes, OLA performance, and employee workloads. A key technical component is the calculation of working time using DAX while accounting for defined business hours, weekends, and public holidays.

## 🎯 Business Objectives

* Monitor ticket volumes and resolution performance over time.
* Calculate working time within defined business hours.
* Exclude weekends and public holidays from working-time calculations.
* Evaluate performance across activity categories, processes, departments, and employees.
* Analyze ticket success and failure rates and review OLA-related performance.
* Identify time-intensive activities and differences in workload distribution.
* Provide interactive reporting to support operational monitoring and decision-making.

## 🛠️ Tools & Technologies

* **Power BI** — Interactive dashboards and reporting
* **DAX** — Working-time calculations, dynamic measures, and performance metrics
* **Data Modeling** — Organizing data to support cross-page analysis
* **Data Visualization** — Presenting operational KPIs and performance trends
* **Interactive Filtering** — Date-based and activity-based filtering

## 📈 Dashboard Pages

### 1. Home Dashboard

Provides a high-level overview of ticket performance, including:

* Monthly and yearly ticket volume
* Ticket success and failure rates
* Total number of tickets
* Average ticket resolution time
* Time-based performance analysis

### 2. Management Dashboard

Supports management-level monitoring through:

* Ticket success rates by year and month
* Ticket volume and resolution performance
* High-level operational performance indicators

### 3. Activity Analysis

Evaluates operational performance across processes, departments, and activity categories.

Key metrics and visualizations include:

* Average working time by process type
* Total ticket volume and working time
* Ticket success and failure rates
* Ticket volume and average resolution time by activity category
* OLA-based success and failure analysis
* Dynamic categorization of activities based on ticket volume

### 4. Employee Analysis

Provides insights into employee workload and performance, including:

* Employee success and failure rates
* Average working time
* Ticket categories handled by each employee
* Resolution performance across activity categories
* Employee workload and productivity comparisons

## 💡 Key Performance Indicators (KPIs)

The dashboard brings together operational KPIs to evaluate ticket resolution performance, working time, workload distribution, and employee productivity.

* **Total Ticket Volume:** Tracks the number of tickets across selected periods and activity categories.
* **Ticket Success Rate:** Measures the percentage of successfully completed tickets and supports performance comparisons over time.
* **Ticket Failure Rate:** Measures the proportion of unsuccessful tickets and helps identify areas requiring further investigation.
* **Average Working Time:** Measures the average working time required to resolve tickets while accounting for defined business hours, weekends, and public holidays.
* **Total Working Time:** Shows the accumulated working time associated with ticket resolution.
* **Employee Workload and Performance:** Combines ticket volume, average working time, and resolution success rates to compare employee workloads and outcomes.
* **Activity and Department Performance:** Compares ticket volumes, resolution times, and success rates across activity categories, processes, and departments.
* **Monthly and Yearly Trends:** Tracks changes in ticket volume and resolution outcomes to identify operational patterns.

### OLA Performance

The dashboard includes visualizations for ticket success and failure based on OLA categories or targets. This analysis helps assess operational performance against the defined criteria represented in the dataset.

A formal **OLA Compliance Rate** should be reported as a separate KPI only when the data model provides sufficient information to determine whether each ticket met its applicable OLA target.

## ⌚ Working Time Calculation with DAX

One of the main technical challenges in this project was calculating working time while accounting for business hours, weekends, and public holidays.

The calculation logic was structured into four stages:

1. **Start Time Adjustment:** Adjusting the ticket start time to account for the beginning of the working day (8:00 AM).
2. **End Time Adjustment:** Adjusting the ticket end time to account for the end of the working day (5:00 PM).
3. **Non-Working Day Exclusion:** Accounting for weekends and public holidays occurring between the start and end dates.
4. **Final Working Time Calculation:** Combining the relevant time intervals to calculate the effective working duration.

This approach distinguishes working time from elapsed calendar time and provides a more meaningful basis for comparing ticket resolution performance.

## 🧮 DAX Measures & Dynamic Categorization

DAX is used to calculate and analyze:

* Total ticket volume
* Average ticket resolution time
* Total working time
* Ticket success and failure rates
* Dynamic measures for activity-volume categories
* Performance metrics across dates, departments, processes, and employees

Dynamic activity categorization groups ticket volumes into configurable ranges, making it easier to compare workload and performance across different activity groups.

## Operational Analysis & Business Value

By combining ticket volume, working time, and resolution outcomes, the dashboard supports several useful business analyses:

* **Workload vs. Success Rate:** Examine whether changes in ticket volume coincide with changes in resolution performance.
* **Working Time vs. Resolution Outcomes:** Compare average working time and success rates across activity categories and processes.
* **Department Performance:** Identify differences in ticket volume, average resolution time, and success rates between departments.
* **Activity Category Analysis:** Identify categories that account for a large share of tickets or require more working time.
* **Employee Performance Comparison:** Compare employee workload, average working time, and resolution outcomes rather than relying on ticket counts alone.
* **Time-Based Trend Analysis:** Examine monthly and yearly changes in ticket volume and resolution performance.

These analyses help highlight areas that may require further investigation and support more informed operational decisions. They do not, by themselves, establish the causes of performance differences.

## Interactive Features

* Year, month, and day filters
* Activity category filters
* Activity type filters
* Cross-page interactive analysis
* Refresh button for updating the report

## Key Skills Demonstrated

* Power BI dashboard development
* DAX measure development
* Working-time calculations with business-hour constraints
* Weekend and public-holiday handling
* KPI development and performance monitoring
* Operational and employee performance analysis
* Dynamic categorization and interactive reporting
* Data visualization for business decision support

---

## 📷 Dashboard Preview

### Home Dashboard

(screenshots/home.png)

### Management Dashboard

(screenshots/management.png)

### Activity Analysis

(screenshots/activity-analysis.png)

### Employee Analysis

(screenshots/employee-analysis.png)

---

## 📁 Project Structure

```text
ticket-performance-power-bi/
├── README.md
├── dashboard/
│   └── Ticket_Performance_Dashboard.pbix
└── screenshots/
    ├── home.png
    ├── management.png
    ├── activity-analysis.png
    └── employee-analysis.png
```
