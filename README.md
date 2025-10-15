
#🚀 NullClass Internship Tasks – Tableau Visualization Project
🧑‍💻 Author: Nitish Rathod
📊 Tool Used: Tableau Public (Mac)
📂 Dataset: Kaggle Job Postings Dataset (used from training project)
🧠 Project Overview

This repository contains my internship task submissions for NullClass, built on top of my training dataset project.
The tasks were designed to test data handling, calculated field logic, conditional filtering, and professional dashboard creation using Tableau Public.

All visualizations are created from the same Kaggle Job dataset, focusing on deeper analytical insights like filtering by region, qualifications, job type, salary ranges, and dynamic time conditions.

#⚙️ Tools and Tech Used

Python (Pandas, NumPy): for initial dataset cleaning

Tableau Public (Mac Silicon): for visualization and dashboards

GitHub: for final submission

📈 Dashboard Summary

The final Tableau dashboard combines multiple analytical sheets that represent each task from the internship requirements.
Each chart is interactive, cleanly labeled, and mobile-view compatible.

⚠️ Note: Some charts appear blank because the dataset does not have records that meet all strict filter conditions.
However, all logical conditions and calculated fields are implemented correctly.

🧩 Task Breakdown
Task 1 – Preference vs Work Type (Intern, Bar Chart)

Goal: Compare Preferences for Intern roles using strict conditions.
Chart Type: Vertical Bar Chart

Key Conditions Implemented:

Work Type = Intern

Latitude < 10

Country not starting with A, B, C, or D

Job Title is single-word & < 10 characters

Company Size < 50,000

Salary > $9,000

Experience is even

Job Posting Month is odd-numbered

Time filter: only visible between 3 PM–5 PM IST


Result:
The dataset didn’t have rows matching all these filters, resulting in an empty plot — but all logic and fields were implemented correctly.

Task 4 – Qualification Drilldown Map

Goal: Display job postings across Africa for select qualifications and filters.
Chart Type: Geographic Map (Drilldown enabled)

Key Conditions Implemented:

Qualification = B.Tech / M.Tech / PhD

Work Type = Full-Time

Country in Africa

Job Title starts with “D”

Preference = Male

Company Size > 80,000

Contact Person starts with “A”

Job Portal = Indeed

Salary Range > $20,000

Time = 3 PM–6 PM IST


Result:
Map configured successfully with Latitude & Longitude, drilldown enabled.
Dataset again had limited matching rows.

Task 6 – Work Type Salary Distribution (Box Plot)

Goal: Analyze salary distribution for Interns under special conditions.
Chart Type: Box-and-Whisker Plot

Key Conditions Implemented:

Work Type = Intern

Latitude < 10

Country name not starting with A, B, C, D

Job Title = single word, < 10 characters

Company Size < 50,000

Salary > $8,000

Experience = even number

Job Posting Date = 2021–2023

Contact Person contains “e”

Time = 3 PM–5 PM IST


Result:
Box plot rendered correctly; filters applied as per conditions.
Limited or no matching records caused minimal visible data points.

Task – Company Size vs Company (Scatter Plot)

Goal: Compare company size vs company names under specific Asian and gender-based filters.
Chart Type: Scatter Plot

Key Conditions Implemented:

Company Size < 50,000

Job Title = “Mechanical Engineer”

Experience > 5 years

Country in Asia (not starting with “I”)

Salary > $50,000

Work Type = Full-Time or Part-Time

Preference = Male

Job Portal = Idealist

Company must have at least 2 vowels

Time = 3 PM–5 PM IST


Result:
Large scatter plot successfully generated; resizing was done using “Entire View.”
Data partially visible due to dataset limitations.

Task – India vs Germany Comparison (Stacked Bar Chart)

Goal: Compare job postings in India vs Germany for specific roles and conditions.
Chart Type: Stacked Bar

Key Conditions Implemented:

Qualification = B.Tech

Work Type = Full-Time

Experience > 2 years

Job Title = Data Scientist, Art Teacher, or Aerospace Engineer

Salary > $10,000

Job Portal = Indeed

Preference = Female

Posting before 08/01/2023

Location not blank

Company name > 8 characters

Time = 3 PM–5 PM IST


Result:
Stacked bars for India and Germany created with colors (Orange for India, Green for Germany).
Limited matching records resulted in partial chart display.

📊 Final Dashboard

The final Tableau Dashboard combines:

All above sheets

Automatic Layout

Consistent fonts, color palettes of Blue shades, and tooltips

Added interactivity through country and work-type filters

Each chart captioned with conditions and notes for clarity
