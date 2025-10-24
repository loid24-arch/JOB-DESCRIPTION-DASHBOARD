🚀 NullClass Internship Tasks – Tableau Visualization Project
🧑‍💻 Author: Nitish Rathod
📊 Tool Used: Tableau Public (Mac)
📂 Dataset: Kaggle Job Postings Dataset (used from training project) 
🔗[Link of Data Set][https://www.kaggle.com/datasets/ravindrasinghrana/job-description-dataset]

🧠 Project Overview

This repository contains my 6 Tableau visualization tasks completed as part of the NullClass Internship.
All tasks are built on the same cleaned Kaggle Job Dataset I used during my training phase.
Each task involves applying advanced filtering, logic-based calculated fields, and professional-level visualization design in Tableau Public.

I’ve also used Python (Pandas + NumPy) for cleaning the dataset before importing it into Tableau.

⚠️ Some charts appear blank due to the dataset not containing records that meet all the strict conditions —
however, every single filter and calculated field is correctly implemented.

⚙️ Tools & Technologies Used

Python: Data cleaning using Pandas & NumPy

Tableau Public (Mac Silicon): Data visualization

GitHub: For project documentation and report submission

📊 Dashboard Summary

All six tasks have been added as separate sheets inside one final interactive dashboard.
The dashboard is well-organized, clean, mobile-friendly, and includes filters for interactivity.
Each chart has its title, tooltips, and captions mentioning its filters and logic.

🧩 Task Breakdown
🟧 Task 1 – Preference vs Work Type (Intern, Bar Chart)

Goal:
Show a comparison between Preference and Work Type for internship roles with multiple filters.

Chart Type: Bar Chart

Conditions Implemented:

Work Type = "Intern"

Latitude < 10

Country name not starting with A, B, C, or D

Job Title must be single-word and < 10 characters

Company Size < 50,000

Salary > $9,000

Experience is an even number

Job Posting Month = odd-numbered month

Time range = 3 PM–5 PM IST

Sorted bars in descending order by count

Result:
All logic applied successfully; dataset couldn’t satisfy all filters, hence the chart may appear empty — which is expected.

🟩 Task 2 – Company Size vs Company Name (Scatter Plot)

Goal:
Plot Company Size vs Company Name for Mechanical Engineer roles filtered by multiple conditions.

Chart Type: Scatter Plot

Conditions Implemented:

Company Size < 50,000

Job Title = “Mechanical Engineer”

Experience > 5 years

Country in Asia (not starting with “I”)

Salary > $50,000

Work Type = Full-Time or Part-Time

Preference = Male

Job Portal = Idealist

Company name must have at least 2 vowels

Time range = 3 PM–5 PM IST

Result:
Chart initially appeared empty, later confirmed visible after resizing to Entire View.
Dataset didn’t have enough matching records, but logic and calculated fields are accurate.

🟦 Task 3 – Top 10 Companies (Tree Map)

Goal:
Show a Tree Map of the top 10 companies hiring Data Scientists with the role “Data Engineer” under complex filters.

Chart Type: Tree Map

Conditions Implemented:

Role = “Data Engineer”

Job Title = “Data Scientist”

Exclude Asian countries

Exclude countries starting with “C”

Latitude < 10

Preference = Female

Qualification = B.Tech

Job Posting Date between 01/01/2023 and 06/01/2023

Job Portal = LinkedIn

Company Size ≥ 10,000

Contact Person name ends with a vowel

Time range = 3 PM–5 PM IST

Result:
Tree map created successfully with labels and hover tooltips.
Data availability was limited, but all calculated logic was implemented precisely.

🟨 Task 4 – Qualification Drilldown Map (Map with Click)

Goal:
Map visualization for African job postings with qualifications-based drilldown.

Chart Type: Geographic Map with Drilldown

Conditions Implemented:

Qualification = B.Tech / M.Tech / PhD

Work Type = Full-Time

Country in Africa

Job Title starts with “D”

Preference = Male

Company Size > 80,000

Contact Person starts with “A”

Job Portal = Indeed

Salary Range > $20,000

Time range = 3 PM–6 PM IST

Result:
Map plotted using Latitude & Longitude.
Click-based drilldown was added for detailed job locations.
Chart may appear empty due to dataset constraints but functions correctly.

🟥 Task 5 – India vs Germany Comparison (Stacked Bar)

Goal:
Compare job postings between India and Germany using specific role and qualification filters.

Chart Type: Stacked Bar Chart

Conditions Implemented:

Qualification = B.Tech

Work Type = Full-Time

Experience > 2 years

Job Title = Data Scientist / Art Teacher / Aerospace Engineer

Salary > $10,000

Job Portal = Indeed

Preference = Female

Only postings before 08/01/2023

Location not blank

Company Name length > 8 characters

Time range = 3 PM–5 PM IST

India = Orange, Germany = Green

Result:
Stacked bar chart formatted with country-based color codes.
Data limitations restricted some records, but all filters worked as expected.

🟪 Task 6 – Work Type Salary Distribution (Box Plot)

Goal:
Show salary distribution by Work Type under multiple logical conditions.

Chart Type: Box-and-Whisker Plot

Conditions Implemented:

Work Type = “Intern”

Latitude < 10

Country not starting with A, B, C, D

Job Title single word, < 10 characters

Company Size < 50,000

Salary > $8,000

Experience = even number

Job Posting Date between 2021–2023

Contact Person contains “e”

Time range = 3 PM–5 PM IST

Result:
Box plot rendered successfully with proper whiskers and range.
Filters applied perfectly; chart may have fewer visible points due to data shortage.

🧮 Common Calculated Fields Used Across Tasks
Calculated Field Name	Logic Summary
Latitude_Below_10	Filters out locations above 10° latitude
Country_Not_ABCD	Excludes countries starting with A, B, C, D
Has_2Plus_Vowels	Company names having ≥ 2 vowels
CompanySize_Lt_50000	Filters small-to-mid companies
Experience_Even	Keeps even-numbered experience values
Country_Asia_Not_I	Includes Asian countries not starting with “I”
CompanyName_Len_Gt8	Company names longer than 8 characters
Time_3PM_to_5PM / Time_3PM_to_6PM	Controls visibility by time range
Contact_Starts_A / Contact_Has_e	Filters based on name patterns
Odd_Month_Posting	Keeps postings from odd-numbered months
🧾 Final Dashboard Overview

Combines all 6 tasks into a single interactive Tableau dashboard

Added filter controls for Country, Work Type, and Qualification

Each chart titled and captioned with task number and filter conditions

Used “Entire View” layout for readability

Consistent color scheme and labeling across visuals

🔗 View My Tableau Dashboard on Tableau Public

🧠 Notes & Observations

Some visualizations appear empty due to strict filter conditions combined with limited dataset records.

All filters, logical checks, and calculated fields were applied precisely as per requirements.

The dataset was cleaned using Python before import, ensuring accurate data types for Tableau.

The project highlights proficiency in:

Data transformation using Pandas

Logical condition handling in Tableau Calculated Fields

Visualization design and storytelling with dashboards

🏁 Conclusion

I have Completed the project But some of the visuals are empty because of the strict filters in the Tasks . 

Clean, professional dashboard design

Ability to interpret and implement complex data-driven tasks

Even with limited dataset support, every visualization and filter was created with accuracy and clarity — reflecting a complete understanding of the analytical process.
