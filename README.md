# JOB-DESCRIPTION-DASHBOARD
This project provides an interactive dashboard that empowers users to delve into current job market trends based on their interests or career goals. By leveraging data on job descriptions, it helps users make informed decisions about their job search.
#TASK 1✅#
📊 Task 1 – Company Size vs Company Name (Scatter Plot)
📘 Overview

This visualization explores the relationship between Company Size and Company Name for specific filtered job postings.
It is the first task from my NullClass Internship, built using the same Kaggle Job Dataset used during my training phase.

🧩 Tools & Technologies

Python (Pandas, NumPy) → Data cleaning and preprocessing

Tableau Public → Interactive visualization and dashboard design

GitHub → Hosting project files and documentation

🧹 Data Preparation

Cleaned raw Kaggle Job Dataset using Python:
Data Set Used : [
](https://www.kaggle.com/datasets/ravindrasinghrana/job-description-dataset)
Removed null or duplicate entries in Salary and Company Size

Standardized categorical fields (Work Type, Preference, Country names)

Saved the clean dataset as cleaned_CSV_file.csv and imported it into Tableau Public.

🎯 Filtering Criteria Used
Field	Condition / Filter Applied
Company Size	< 50,000
Job Title	Exactly “Mechanical Engineer”
Experience	> 5 years
Country	Located in Asia but not starting with ‘I’
Salary	> $50,000
Work Type	Full-Time or Part-Time
Preference	Male
Job Portal	Idealist
Company Name	Must contain at least 2 vowels
Display Time	Between 3 PM – 5 PM IST,These Filter is not possible in Tableau Public.
📍 Visualization Details

Chart Type: Scatter Plot

X-Axis: Company Name

Y-Axis: Company Size

Color/Shape: Optional (Work Type or Preference)

Tooltips: Company, Salary, Experience, Country

🧮 Calculated Fields Created
Field Name	Purpose
Has_2Plus_Vowels	Returns True if Company Name contains ≥ 2 vowels
Valid_Country	Returns True if Country is in Asia and does not start with “I”
Valid_Time	Restricts display between 3 PM–5 PM IST using NOW() function

Note: The time-based filter may evaluate False outside 3–5 PM IST in Tableau Public, as NOW() is static on load. The logic is implemented correctly for demonstration.

🧭 Insights

Shows how smaller Asian companies hire Mechanical Engineers with experience > 5 years.

Demonstrates advanced filter stacking and string functions within Tableau.

🧱 Dashboard Design

View Mode: Entire View for auto fit

Filters: All above conditions made interactive

Responsive layout with clear labels and tooltips

🌐 Live Dashboard

🔗 View on Tableau Public
 ([](https://public.tableau.com/views/COMPANYSIZEVSCOMPANYMECHASIAIDEALIST/COM_SIZEVSCOM_?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

 # QUALIFICATION MAP 
 🗺️ Task 1 – Qualification Drilldown Map (Interactive Map Visualization)
📘 Overview

This task visualizes job postings based on qualification level and geographical distribution.
It is part of my NullClass Internship Project, extending the Kaggle Job Dataset used during my training.

The map highlights high-salary full-time roles in Africa, filtered by strict professional criteria, and includes a click-based drilldown to view detailed job locations.

🧩 Tools & Technologies

Python (Pandas, NumPy) → for data cleaning and filtering before visualization

Tableau Public (Mac) → for creating interactive maps and dashboards

GitHub → for hosting project files and documentation

🧹 Data Preparation

The Kaggle Job Dataset was preprocessed in Python:

Removed missing or invalid entries in key fields (Salary, Latitude, Longitude, etc.)

Normalized text case for Job Title, Qualification, and Country fields

Filtered only countries located within the African continent

Saved cleaned data as cleaned_jobs_africa.csv for Tableau import

🎯 Filtering & Logical Conditions
Condition	Criteria
Qualification	B.Tech, M.Tech, or PhD
Work Type	Full-Time
Country	Must be in Africa (other continents ignored)
Job Title	Must start with “D” (e.g., “Data Engineer”, “Design Analyst”)
Preference	Male
Company Size	> 80,000
Contact Person	Must start with “A”
Job Portal	Indeed
Salary Range	> $20,000
Display Time	Between 3 PM – 6 PM IST , Unimplementable in Taleau Public
📍 Visualization Details

Chart Type: Map with interactive drilldown

Plotted Using: Latitude (Y-axis) and Longitude (X-axis)

Drilldown Behavior: Clicking on any map point reveals city-level job details and salary info.

Map Layers:

Company location markers

Tooltips showing Company Name, Qualification, Job Title, Salary Range

🧮 Calculated Fields Created
Field Name	Description
Valid_Qualification	Checks if qualification is one of B.Tech, M.Tech, or PhD
Starts_With_D	Filters Job Title beginning with “D”
Starts_With_A	Filters Contact Person beginning with “A”
High_Salary	Keeps records where Salary Range > $20,000
Valid_Time	Allows display only between 3 PM – 6 PM IST , Unsuccessfull
In_Africa	Validates if country is located in Africa (based on continent mapping)
⚙️ Technical Notes

Time filter may appear as “False” outside 3–6 PM IST since Tableau Public doesn’t update NOW() dynamically.

For demonstration, a mock TRUE filter was used to keep the dashboard visible.

Drilldown behavior is implemented using Tableau’s “Go to Sheet” on Click action.

🧭 Insights

Identifies major African hubs for high-paying engineering roles.

Enables drilldown exploration of company-specific data per qualification.

Demonstrates advanced Tableau skills like filters, calculated fields, and drill-through navigation.

🧱 Dashboard Design

Layout: “Entire View” (responsive for all screens)

Base Map: Tableau Light Theme

Filters on Dashboard: Qualification, Country, Salary, Work Type

Tooltip includes: Company Name, Job Title, Salary Range, and Qualification

🌐 Live Dashboard

🔗 View on Tableau Public
 [](https://public.tableau.com/shared/QF2BT6F9M?:display_count=n&:origin=viz_share_link)
