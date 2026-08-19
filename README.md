# HR Analytics & Workforce Insights Dashboard

## 📌 Project Overview
This repository contains an end-to-end HR Analytics Report built in Power BI. The dashboard provides a concise summary of headcount, retention, and turnover metrics[cite: 4]. Designed for HR professionals, this tool offers a comprehensive overview of workforce dynamics, enabling teams to identify attrition patterns and develop targeted strategies for talent retention and engagement[cite: 4].

## 📊 Dashboard Features
The interactive dashboard is separated into three primary analytical views:

### 1. Headcount Analysis
Provides a snapshot of the current workforce (e.g., 2,796 employees as of 2019) broken down by various demographics[cite: 4].
*   **Demographic Breakdown:** Visualizes headcount by Gender, Age, Race & Ethnicity, Education Level, and Marital Status[cite: 4].
*   **Organizational Breakdown:** Displays employee distribution across Departments (e.g., Software, Sales, HR) and Job Levels (Individual Contributor to CEO)[cite: 4].
*   **Location:** Tracks the ratio of On-site vs. Remote employees[cite: 4].
*   **Custom Tooltips:** Features a specialized tooltip enabling deep-dive analysis of the Top/Bottom 20 salary earners within specific departments or cities[cite: 4].

### 2. Employee Retention
Analyzes how well the company is retaining its talent over a selected timeframe[cite: 4].
*   **Retention Metrics:** Highlights the overall retention rate (e.g., 83.6% for 2013-2019), tracking starting and ending headcounts[cite: 4].
*   **Trend Tracking:** Features line charts comparing year-over-year retention changes by Education Level[cite: 4].
*   **Segmented Retention:** Breaks down retention success by Job Level and Department to pinpoint areas with the highest loyalty[cite: 4].

### 3. Employee Turnover
Explores the reasons and trends behind employee departures[cite: 4].
*   **Turnover Metrics:** Displays total turnover percentage alongside the exact count of departing employees and the average number of active employees[cite: 4].
*   **Detailed Roster:** A comprehensive table logging departing employees, their termination date, department, and total salary[cite: 4].
*   **Attrition Drivers:** Analyzes turnover by Termination Type (Involuntary vs. Voluntary 19%/81% split) and tracks specific Termination Reasons (e.g., More flexible benefits, Found a better opportunity, Better salary)[cite: 4].

## 🗂️ Dataset Dictionary
This project relies on two core datasets containing employee demographic and historical employment records. 

### `people_data.csv`
Contains static demographic and location information for employees.
*   `employee_id`: Unique identifier for the employee.
*   `gender`: Employee's identified gender.
*   `race`: Employee's racial/ethnic identification.
*   `birth_date`: Employee's date of birth.
*   `education`: Highest degree or level of education completed.
*   `location`: Indicator of remote or on-site work.
*   `location_city`: City where the employee is based.
*   `marital_status`: Marital status of the employee.
*   `employment_status`: Current status of employment.

### `people_employment_history.csv`
Contains organizational, financial, and lifecycle records.
*   `employee_id`: Unique identifier tying back to demographic data.
*   `first_name` / `last_name`: Employee name.
*   `department` / `sub-department`: Organizational placement.
*   `first_level_manager` through `fourth_level_manager`: Reporting hierarchy.
*   `job_level`: Seniority or tier of the employee's role.
*   `salary`: Current or final compensation.
*   `hire_date`: Date the employee joined the company.
*   `term_date`: Date the employee left the company (if applicable).
*   `term_type`: Categorization of departure (Voluntary/Involuntary).
*   `term_reason`: Specific reason for leaving.
*   `active_status`: Indicator of whether they are currently employed.

## 🚀 Getting Started
1. Clone this repository to your local machine.
2. Ensure you have [Power BI Desktop](https://powerbi.microsoft.com/desktop/) installed.
3. Open the `.pbix` file.
4. Ensure the data sources point correctly to the local `people_data.csv` and `people_employment_history.csv` files, and click **Refresh** to load the data.

## 🤝 Acknowledgments
*   Dashboard design and layout inspired by **Sweatpants BI**[cite: 4].
