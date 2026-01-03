# Vaccination-Data-Analysis-and-Visualization
Analyze global vaccination data to understand trends in vaccination coverage, disease incidence, and effectiveness. Data will be cleaned, and stored in a SQL database. Power BI will be used to connect to the SQL database and create interactive dashboards that provide insights on vaccination strategies and their impact on disease control
## Business Use Cases:
●	Public Health Strategy:
○	Assess the effectiveness of vaccination programs in different regions and populations.
○	Prioritize areas with low vaccination coverage for targeted interventions.
●	Disease Prevention:
○	Identify diseases with high incidence rates despite vaccination efforts, suggesting vaccine inefficacies or areas for improvement.
○	Support policies on booster vaccines or new vaccine introductions.
●	Resource Allocation:
○	Determine regions with low vaccination coverage and plan targeted resource distribution to improve vaccination rates.
○	Forecast vaccine demand based on current trends for better supply chain management.
●	Global Health Policy:
○	Provide data-driven recommendations for vaccination policy formulation.
○	Support governments and health organizations with evidence on vaccine effectiveness.
## Approach:
### Data Cleaning.
●	Handle Missing Data: Impute missing values or remove incomplete records.
●	Normalize Units: Ensure consistency in units across datasets (e.g., percentage of coverage, number of reported cases).
●	Date Consistency: Format date fields uniformly across tables for easier analysis.
###  SQL Database Setup
●	Create Tables: Store the extracted and cleaned data into relational SQL tables (e.g., vaccination data, disease incidence data, antigen data).
●	Normalize Data: Structure the data into separate tables (e.g., vaccines, diseases, countries, years) to avoid redundancy and improve querying performance.
●	Data Integrity: Implement primary and foreign keys to ensure referential integrity.
### Power BI Integration. 
●	Connect Power BI to SQL Database:
○	Use Power BI’s SQL connector to link to the SQL database and pull in the relevant tables for analysis.
○	Set up scheduled refreshes for updated data.
### Data Visualization in Power BI
●	Create Interactive Dashboards:
○	Use Power BI to create dynamic and visually engaging reports with filters and slicers for users to explore the vaccination data.
○	Visualize vaccination rates, disease incidence, and antigen coverage over time and across regions.
●	Key Visualizations:
○	Geographical Heatmaps: Display vaccination coverage and disease incidence by region.
○	Trend Lines/Bar Charts: Show trends in vaccination coverage, disease rates, and effectiveness over multiple years.
○	Scatter Plots: Correlate vaccination coverage and disease incidence across different countries or regions.
○	KPI Indicators: Track progress toward vaccination goals and health targets.

### Exploratory Data Analysis (EDA):
●	Analyze vaccination coverage, disease incidence trends, and regional disparities using statistical summaries and correlation analysis. Visualize insights with bar charts, heatmaps, and line graphs to identify patterns, highlight low-coverage areas, and assess the impact of vaccination on disease reduction.

## Data Set Explanation:
### Table 1 : coverage data
Variables:
●	Group: Categorization of the data. Here, it represents countries.
●	Code: Unique identifier for the country (ISO Alpha-3 code).
●	Name: Name of the country.
●	Year : The year the data is recorded for.
●	Antigen: Vaccine identifier or code.
●	Antigen_description: Full description of the vaccine.
●	Coverage_category: Type of coverage reported, such as administrative or official.
●	Coverage_category description: Expanded details of the coverage category.
●	Target number: Number of individuals targeted for vaccination.
●	Dodge: Number of doses administered.
●	Coverage: Percentage of the target population that was vaccinated.
### Table 2 : Incidence Rate
Variables:
●	Group : Classification of the data; here, it represents countries.
●	Code: Unique identifier for the country (ISO Alpha-3 code).
●	Name: Name of the country.
●	Year: The year the data is recorded for.
●	Disease: Code or short name of the disease.
●	Disease description: Full description of the disease.
●	Denominator: The population basis used to calculate the incidence rate (e.g., per live births, per total population).
●	Incidence rate: Number of disease cases per specified population unit.

### Table 3 : Reported cases
Variables:
●	Group : Classification of the data; here, it represents countries.
●	Code: Unique identifier for the country (ISO Alpha-3 code).
●	Name: Name of the country.
●	Year: The year the data is recorded for.
●	Disease: Code or short name of the disease.
●	Disease description: Full description of the disease.
●	Cases: Number of reported cases of the disease for the specified year and region.

### Table 4 : Vaccine Introduction
Variables:
●	ISO_3_Code : Unique 3-letter ISO country code.
●	Country Name: Name of the country.
●	Who Region: World Health Organization (WHO) region to which the country belongs.
●	Year: The year the data is recorded for.
●	Description: Name of the vaccine or vaccine type.
●	Intro: Indicates whether the vaccine has been introduced into the country's vaccination program.
### Table 5 :  Vaccine Schedule Data
Variables:
●	ISO_3_Code : Unique 3-letter ISO country code.
●	Country Name: Name of the country.
●	Who Region: World Health Organization (WHO) region to which the country belongs.
●	Year: The year the data is recorded for.
●	Vaccine code: Code for the vaccine.
●	Vaccine description: Name and details of the vaccine.
●	Schedule rounds: The dose or round of the vaccine in the schedule.
●	Target pop: Specific population targeted for the vaccine dose.
●	Target pop description: Detailed description of the target population.
●	Geoarea: Geographic area of administration.
●	Age administered: Age or time of vaccine administration.
●	Source comment: Additional information or context for administration.



