# Data Jobs Dashboard – Power BI Project

![Dashboard Page 1](/Images/Page_1.png)

## Project Overview

This Power BI dashboard analyzes data-related job postings using a flat job postings dataset. The report is designed to help users explore job market trends, compare salary patterns across different data roles, and drill into specific job titles for deeper analysis.

The dashboard includes a high-level overview page and a dedicated drill-through page. Together, they provide both summary-level insights and detailed role-level breakdowns.

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

The dataset appears to contain job posting information for data-related roles, including salary details, job type, location, posting platform, and benefit-related indicators.

**Note:** The original dataset file is not included in this repository because it exceeds GitHub's 100 MB file size limit.

---

## Report Pages

### 1. Data Jobs Dashboard

![Dashboard Page 1](/Images/Page_1.png)

This is the main dashboard page. It provides an overall view of the data jobs market using KPI cards, trend analysis, salary comparisons, and summary tables.

#### Main Visuals

**KPI Cards**

The top section includes four card visuals showing key metrics:

- Minimum/selected job title from `job_title_short`
- Rating from `rating`
- Average yearly salary from `salary_year_avg`
- Average hourly salary from `salary_hour_avg`

These cards give users a quick snapshot of the dataset and salary indicators.

**Job Posting Trend by Month**

A line chart shows the count of job postings over time using:

- Month from `job_posted_date`
- Count of `job_title_short`

This visual helps identify how job posting volume changes across months.

**Salary and Job Count by Job Title**

A bar chart compares job titles using:

- `job_title_short`
- Average yearly salary
- Count of job postings

This allows users to compare demand and salary levels across different data roles.

**Yearly vs Hourly Salary Comparison**

A scatter chart compares:

- Median yearly salary
- Median hourly salary
- Job title category

This visual helps users understand how salary patterns differ between yearly-paid and hourly-paid job categories.

**Job Title Summary Matrix**

A matrix/pivot table summarizes each job title by:

- Job title
- Quarter from `job_posted_date`
- Average yearly salary
- Average hourly salary
- Posting count sparkline by month

This provides a more detailed tabular breakdown of role-level salary and demand trends.

**Drill-through Button**

The page also contains an action button, likely used to navigate or support drill-through interaction into the detailed job title page.

---

### 2. Job Title Drill Through

![Dashboard Page 2](/Images/Page_2.png)

This page is designed for detailed analysis of a selected job title. It is intended to be accessed from the main dashboard through drill-through functionality.

#### Main Visuals

**Selected Job Title Card**

A large card displays the selected job title using `job_title_short`. This helps the user confirm which role is currently being analyzed.

**Back Button**

A back/action button is included so users can return to the main dashboard after drilling through.

**Yearly Salary Gauge**

A gauge visual analyzes yearly salary using:

- Average yearly salary
- Median yearly salary
- Minimum yearly salary

This shows how the selected role performs in terms of annual salary.

**Hourly Salary Gauge**

A second gauge visual analyzes hourly salary using:

- Average hourly salary
- Median hourly salary
- Minimum hourly salary

This helps compare hourly pay patterns for the selected job title.

**Work From Home Breakdown**

A donut chart shows the distribution of remote/work-from-home availability using:

- `job_work_from_home`
- Count of records

**Degree Requirement Breakdown**

A donut chart analyzes whether job postings mention no degree requirement using:

- `job_no_degree_mention`
- Count of records

**Health Insurance Breakdown**

A donut chart shows whether job postings mention health insurance using:

- `job_health_insurance`
- Count of records

**Job Country Map**

A map visual shows job posting distribution by country using:

- `job_country`
- Count of country records

This provides a geographical view of job posting concentration.

**Schedule Type Treemap**

A treemap shows job posting distribution by schedule type using:

- `job_schedule_type`
- Count of records

This helps compare full-time, part-time, contractor, and other schedule categories where available.

**Job Source Bar Chart**

A bar chart shows where jobs were posted or accessed from using:

- `job_via`
- Count of records

This helps identify the most common job posting platforms or sources.

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

---

## How to Use the Dashboard

1. Open the file in Power BI Desktop.
2. Start from the **Data Jobs Dashboard** page.
3. Review the KPI cards for a quick summary.
4. Use the trend, bar, scatter, and matrix visuals to compare job titles and salary patterns.
5. Right-click a job title or relevant data point and use **Drill through** to open the **Job Title Drill Through** page. Alternatively, use the dedicated drill-through button provided in the dashboard for easier navigation.
6. Use the drill-through page to analyze the selected job title in more detail.
7. Use the back button to return to the main dashboard.

---

## Business Questions Answered

This dashboard helps answer questions such as:

- Which data job titles appear most frequently in the dataset?
- How do average yearly salaries differ by job title?
- How do hourly salaries compare across different roles?
- How does job posting volume change over time?
- Which job titles have stronger salary potential?
- Which countries have the highest concentration of job postings?
- How common are remote jobs in the selected role?
- How often do job postings mention no degree requirement?
- How often is health insurance mentioned?
- Which job platforms or sources appear most often?

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
- Data modeling using a flat table structure
- Business intelligence reporting for job market analytics

---

## Tools Used

- Power BI Desktop
- Power Query / Power BI data model
- DAX aggregations through visual-level calculations
- Interactive Power BI visuals


## Repository Structure Suggestion

```text
PowerBI Dashboards/
│
├── jobs_dashboard.pbix
├── README.md
│
├── Data/
│   └── job_postings_flat.csv
│
└── Images/
    ├── Page_1.png
    └── Page_2.png
```

---

## Project Summary

The Data Jobs Dashboard is an interactive Power BI report focused on analyzing data job postings. The main page provides an overview of job posting trends, salary comparisons, and role-level summaries. The drill-through page allows users to explore a selected job title in more detail, including salary gauges, remote work availability, degree mention, health insurance, country distribution, schedule type, and job source.

This project is suitable for demonstrating beginner-to-intermediate Power BI skills, especially dashboard design, visual selection, drill-through functionality, and job market analytics.
