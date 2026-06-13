# Data Jobs Dashboard – Power BI Project

![Dashboard Page 1](/Images/Page_1.png)

## Project Overview

This Power BI project analyzes data-related job postings using a flat job postings dataset. The report is designed to help users explore job market trends, compare salary patterns across different data roles, identify in-demand skills, and drill into specific job titles for deeper analysis.

The project now includes two dashboard versions:

- **Data Jobs Dashboard 1.0** – the original dashboard with high-level job market, salary, trend, and drill-through analysis.
- **Data Jobs Dashboard 2.0** – an upgraded dashboard focused on cleaner executive-style KPI reporting, interactive slicers, skill demand analysis, and salary comparison by role.

---

## Dashboard Files

- [`jobs_dashboard.pbix`](jobs_dashboard.pbix) – original Power BI dashboard file.
- [`jobs_dashboard_v2.pbix`](jobs_dashboard_v2.pbix) – upgraded Power BI dashboard 2.0 file.

---

## Dataset

The report is built using a single table:

`job_postings_flat`

Key fields used in the dashboard include:

- `job_title_short`
- `job_posted_date`
- `salary_year_avg`
- `salary_hour_avg`
- `rating`
- `job_work_from_home`
- `job_no_degree_mention`
- `job_health_insurance`
- `job_country`
- `job_schedule_type`
- `job_via`
- Skills-related fields used for skill demand analysis

The dataset contains job posting information for data-related roles, including salary details, job type, location, posting platform, benefit-related indicators, and skills.

**Note:** The original dataset file is not included in this repository because it exceeds GitHub's 100 MB file size limit.

---

## Dashboard Image Links

- [Dashboard Page 1](/Images/Page_1.png)
- [Dashboard Page 2 – Drill Through](/Images/Page_2.png)
- [Dashboard Page 3 – Data Jobs Dashboard 2.0](/Images/Page_3.png)

---

## Report Pages

### 1. Data Jobs Dashboard

![Dashboard Page 1](/Images/Page_1.png)

This is the main dashboard page from the original report. It provides an overall view of the data jobs market using KPI cards, trend analysis, salary comparisons, and summary tables.

#### Main Visuals

**KPI Cards**

The top section includes card visuals showing key metrics such as selected job title, rating, average yearly salary, and average hourly salary.

**Job Posting Trend by Month**

A line chart shows the count of job postings over time using `job_posted_date`. This helps identify how job posting volume changes across months.

**Salary and Job Count by Job Title**

A bar chart compares job titles by salary and job count, helping users compare demand and salary levels across different data roles.

**Yearly vs Hourly Salary Comparison**

A scatter chart compares median yearly salary, median hourly salary, and job title category. This helps show how salary patterns differ between yearly-paid and hourly-paid roles.

**Job Title Summary Matrix**

A matrix summarizes each job title by quarter, salary, hourly pay, and posting count trend.

**Drill-through Button**

The page includes a drill-through/action button for navigating into the detailed job title page.

---

### 2. Job Title Drill Through

![Dashboard Page 2](/Images/Page_2.png)

This page is designed for detailed analysis of a selected job title. It is intended to be accessed from the main dashboard through drill-through functionality.

#### Main Visuals

**Selected Job Title Card**

A large card displays the selected job title so users can confirm which role is being analyzed.

**Back Button**

A back/action button allows users to return to the main dashboard after drilling through.

**Yearly Salary Gauge**

A gauge visual analyzes yearly salary using average, median, and minimum yearly salary.

**Hourly Salary Gauge**

A second gauge visual analyzes hourly salary using average, median, and minimum hourly salary.

**Work From Home Breakdown**

A donut chart shows the distribution of remote/work-from-home availability.

**Degree Requirement Breakdown**

A donut chart analyzes whether job postings mention no degree requirement.

**Health Insurance Breakdown**

A donut chart shows whether job postings mention health insurance.

**Job Country Map**

A map visual shows job posting distribution by country.

**Schedule Type Treemap**

A treemap shows job posting distribution by schedule type.

**Job Source Bar Chart**

A bar chart shows where jobs were posted or accessed from.

---

### 3. Data Jobs Dashboard 2.0

![Dashboard Page 3](/Images/Page_3.png)

Dashboard 2.0 is the upgraded version of the report. It uses a cleaner layout, stronger KPI presentation, slicer-based interactivity, and focused analysis around skills and top-paying data roles.

#### Main Visuals

**Interactive Slicers**

The top section includes slicers for:

- Job title
- Country

A **Clear all slicers** button is also included to reset the report filters quickly.

**KPI Cards**

The dashboard includes four main KPI cards:

- Job Count
- Skills Per Job
- Median Yearly Salary
- Median Hourly Salary

These cards give users a quick executive-level summary of the data jobs market.

**Top Skills in Data**

A horizontal bar chart answers the question: **What are top skills in data?**

The visual ranks skills such as Python, SQL, AWS, Azure, Tableau, Spark, R, Excel, Power BI, and Java. It also includes a measure selector so users can switch between:

- Job Count
- Job Percent

This makes the chart more flexible because users can analyze skills by absolute demand or percentage share.

**Top Paying Jobs in Data**

A horizontal bar chart answers the question: **What are top paying jobs in data?**

It compares roles such as Machine Learning Engineer, Software Engineer, Data Engineer, Senior Data Engineer, Cloud Engineer, Senior Data Scientist, Business Analyst, Data Scientist, Senior Data Analyst, and Data Analyst.

The salary selector allows users to switch between:

- Median Hourly Salary
- Median Yearly Salary

This gives users a clearer view of which data roles pay the most depending on the salary type selected.

---

## Dashboard Features

- High-level KPI summary of data job postings
- Monthly job posting trend analysis
- Salary comparison by job title
- Yearly vs hourly salary comparison
- Matrix summary with quarterly and monthly detail
- Drill-through page for selected job titles
- Role-level salary gauges
- Remote work, degree requirement, and health insurance breakdowns
- Geographic job distribution through map visualization
- Job source and schedule type analysis
- Dashboard 2.0 with improved layout and visual design
- Job title and country slicers
- Clear all slicers reset button
- Top skills analysis by job count and job percent
- Top-paying jobs analysis by median hourly and yearly salary

---

## How to Use the Dashboard

1. Open the Power BI file in Power BI Desktop.
2. Use `jobs_dashboard.pbix` for the original dashboard and drill-through report.
3. Use `jobs_dashboard_v2.pbix` for the upgraded Dashboard 2.0 version.
4. Start from the main dashboard page to review the KPI cards and overall market trends.
5. Use slicers to filter by job title or country.
6. Use the skill measure selector to switch between job count and job percent.
7. Use the salary type selector to switch between median hourly salary and median yearly salary.
8. In the original dashboard, right-click a job title or relevant data point and use **Drill through** to open the **Job Title Drill Through** page.
9. Use the back button to return to the main dashboard.

---

## Business Questions Answered

This dashboard helps answer questions such as:

- Which data job titles appear most frequently in the dataset?
- How do average and median salaries differ by job title?
- How do hourly salaries compare across different roles?
- How does job posting volume change over time?
- Which job titles have stronger salary potential?
- Which countries have the highest concentration of job postings?
- How common are remote jobs in the selected role?
- How often do job postings mention no degree requirement?
- How often is health insurance mentioned?
- Which job platforms or sources appear most often?
- Which skills are most in demand for data jobs?
- Which skills appear most often by job count and percentage share?
- Which data roles offer the highest median hourly salary?
- Which data roles offer the highest median yearly salary?

---

## Skills Demonstrated

This Power BI project demonstrates:

- Dashboard design and visual storytelling
- KPI card creation
- Time-series analysis
- Salary analysis
- Drill-through report navigation
- Use of map, gauge, donut, treemap, scatter, bar, line, and matrix visuals
- Role-level filtering and interactivity
- Slicer setup and slicer reset button design
- Field parameter/measure selector style reporting
- Skill demand analysis
- Median salary analysis
- Data modeling using a flat table structure
- Business intelligence reporting for job market analytics

---

## Tools Used

- Power BI Desktop
- Power Query / Power BI data model
- DAX aggregations and measures
- Interactive Power BI visuals
- Slicers and report navigation buttons

---

## Repository Structure Suggestion

```text
PowerBI Dashboards/
│
├── jobs_dashboard.pbix
├── jobs_dashboard_v2.pbix
├── README.md
│
├── Data/
│   └── job_postings_flat.csv
│
└── Images/
    ├── Page_1.png
    ├── Page_2.png
    └── Page_3.png
```

---

## Project Summary

The Data Jobs Dashboard is an interactive Power BI report focused on analyzing data job postings. The original dashboard provides an overview of job posting trends, salary comparisons, and role-level summaries, while the drill-through page allows users to explore a selected job title in more detail.

Dashboard 2.0 improves the project by adding a cleaner executive-style design, job title and country slicers, a clear slicer reset button, stronger KPI cards, top skills analysis, and top-paying job comparisons using median hourly and yearly salary.
