# Data Professional Survey Breakdown (Power BI)

## Project Overview
This project involves conducting a comprehensive analysis of a real-world survey dataset collected from data professionals across various platforms like LinkedIn and Twitter. The primary goal was to transform raw survey responses into an interactive **Power BI dashboard**, providing key insights into the demographics, career sentiments, and skill preferences within the data professional landscape. This analysis helps in understanding industry trends and informing career decisions for aspiring and current data professionals.

## Dataset
The project utilized a real CSV file downloaded directly from the survey website.  
- **Respondents:** Approximately 600-700 individuals (630 survey takers counted in the final dashboard).  
- **Key Fields / Survey Questions (examples):**
  - **Unique ID:** Unique identifier for each survey taker.  
  - **Email:** Collected for anonymity, but not used for analysis.  
  - **Date Taken:** When the survey was completed.  
  - **Job Title:** "Which title fits you best in your current role?" (Data Analyst, Architect, Engineer, Scientist, Database Developer, Other, Student, None). This field required significant cleaning due to many "Other, please specify" entries.  
  - **Current Yearly Salary:** Provided as ranges (e.g., "106-125k"), transformed into numerical averages for analysis.  
  - **Industry:** Industry of the professional.  
  - **Favorite Programming Language:** Multiple-option question.  
  - **Happiness Ratings:** Rated 0-10 for aspects like Salary, Work-Life Balance, Co-workers, Management, Upward Mobility, Learning New Things.  
  - **Difficulty Breaking Into Data:** Categorical responses (e.g., Very Difficult, Easy).  
  - **Looking for a New Job:** Reasons such as remote work, better salary.  
  - **Demographics:** Male/Female, Country, Age.

## Tools Used
- **Microsoft Power BI Desktop:** For data connection, transformation, modeling, DAX calculations, visualization, and dashboard creation.  
- **Power Query Editor:** Embedded within Power BI for robust data cleaning and transformation.

## Methodology / Steps Taken
1. **Data Connection & Initial Load:** Connected Power BI Desktop to the raw CSV data source.  
2. **Data Transformation with Power Query:**  
   - Removed unnecessary columns to streamline the dataset.  
   - Standardized job titles by splitting "Other, please specify" entries into consistent categories (Analyst, Architect, Engineer, Data Scientist, Database Developer, Other, Student/None).  
   - Cleaned "Current Yearly Salary" ranges by creating a numeric **Average Salary**.  
   - Transformed age ranges into consistent numeric values.  
   - Verified and corrected data types for all relevant columns.  
3. **Dashboard Design & Visualization:**  
   - Title: **Data Professional Survey Breakdown**  
   - Custom theme and background.  
   - **KPI Cards:**  
     - Count of Survey Takers: 630  
     - Average Age: ~30 years  
   - **Stacked Bar Chart:** Average salary by job title (Data Scientists highest, ~$93k).  
   - **Clustered Column Chart:** Favorite programming languages (Python most popular).  
   - **Treemap:** Distribution of survey takers by country, highlighting salary differences.  
   - **Gauge Charts:** Happiness ratings for Work-Life Balance (~5.74/10) and Salary.  
   - **Donut Chart:** Average salary comparison by gender.  
   - **Filled Map / Categorical Chart:** Difficulty breaking into the data industry.  
   - Layout organized for clarity with proper titles, labels, and sizing.  

## Key Results & Insights
- **Demographic Snapshot:** 630 respondents, average age ~30 years.  
- **Salary Trends by Role:**  
  - Data Scientists: ~$93k  
  - Data Engineers: ~$65k  
  - Data Architects: ~$63k  
  - Data Analysts: ~$55k  
- **Geographical Salary Variations:** Higher salaries in the United States than in India due to cost-of-living differences.  
- **Popular Programming Languages:** Python overwhelmingly preferred.  
- **Work-Life Balance vs. Salary Satisfaction:** Moderate work-life balance satisfaction (5.74/10), lower salary satisfaction.  
- **Gender-based Salary Comparison:** Dashboard allows comparison of average salaries between male and female respondents.  
- **Breaking Into Data:** Visualizes perceived difficulty across survey participants.  
- **Interactive Exploration:** Users can filter by country, job title, and other demographics to explore customized insights.

## Technical Skills Demonstrated
- **Power BI Desktop:** End-to-end dashboard creation and layout.  
- **Power Query Editor:** Advanced data cleaning (splitting columns, creating custom columns, changing data types).  
- **DAX (Data Analysis Expressions):** Aggregations for key metrics (Average, Count).  
- **Data Modeling:** Preparing complex datasets for analysis.  
- **Visualization Design:** Card, Stacked Bar, Clustered Column, Treemap, Gauge, Donut, Filled Map.  
- **Interactive Dashboard Features:** Slicers, filters, and interactive elements for exploration.  
- **Data-Driven Storytelling:** Translating raw survey data into actionable insights.

## Future Enhancements
- Further clean "Other, please specify" responses and programming language categories.  
- Develop advanced DAX measures for comparative analysis (e.g., salary index by country factoring cost-of-living).  
- Integrate additional survey questions for multi-dimensional insights.  
- Create multi-page dashboards with drill-through capabilities for granular analysis.
