**This project showcases a comprehensive Human Resources (HR) data analysis using Power BI, designed to monitor workforce metrics and provide actionable insights into the core drivers of employee attrition.**

## Project Goals
The primary objectives of this analysis were:
- Monitor key HR metrics such as total employees, active/inactive counts, and turnover trends.
- Understand which organizational, demographic, and performance factors have the highest correlation with employee attrition.

## Data Modeling and Preparation
* Source: Data was sourced directly from GitHub using Power BI's Web Connector.
* Structure: Snowflake schema was implemented using Dim (Dimension) and Fact (Fact) tables, linked by relationships.
* Key Transformations:
    * Used Power Query to create clear Age Bins for grouping demographic data.
    * A dedicated calculated table (DimDate) was created in DAX to enable sophisticated temporal analysis.
* All core business logic was consolidated into an organized _Measures table. 
* Extensive use of CALCULATE and USERELATIONSHIP to manage inactive relationships and calculate metrics based on different date contexts.

![WhatsApp Image 2025-12-15 at 5 10 26 PM](https://github.com/user-attachments/assets/ac26bd0d-ac90-47b4-9d6d-7dab54ca64a4)


## Key Business Insights
- Overall Attrition: The company maintains an overall attrition rate of 16.1%.
- High-Risk Roles: Attrition is critically high in two specific roles:
  - Sales Representative (39.8% attrition rate) 
  - Recruiter (37.5% attrition rate) 
- Environmental Factors: Employees are significantly more likely to leave if they are:
  - Required to work OverTime.
  - Designated as a Frequent Traveller.
- Tenure Risk: Retention efforts should be heavily focused on new hires, as the highest attrition occurs within the first 0 to 2 years of employment.
- Performance Tracking: Year-over-year analysis reveals fluctuations in key metrics like Job Satisfaction and Manager Rating, necessitating continuous monitoring to preempt engagement issues.

## Overview Page
This page provides the high-level status of the workforce and tracks core HR operational metrics.

<img width="880" height="496" alt="Screenshot 2025-12-15 at 5 01 11 PM" src="https://github.com/user-attachments/assets/6d9ab847-b1fd-4f23-bf35-0977afc75bdf" />

## Demographics Page
This page profiles the employee base, analyzing age, gender, marital status, and compensation across different groups.

<img width="879" height="495" alt="Screenshot 2025-12-15 at 5 01 32 PM" src="https://github.com/user-attachments/assets/c414d204-3369-4602-8a29-2bac63ae655b" />

## Performance Tracker Page
This page is designed for deep dives into individual employee performance and satisfaction history, with a focus on historical trends.

<img width="876" height="493" alt="Screenshot 2025-12-15 at 5 01 46 PM" src="https://github.com/user-attachments/assets/3b903902-b53b-4719-a8b8-937056e4aff5" />

## Attrition Page
This page isolates the primary factors driving employee turnover, which is critical for formulating retention strategies.

<img width="875" height="492" alt="Screenshot 2025-12-15 at 5 02 03 PM" src="https://github.com/user-attachments/assets/3a798efc-1eda-4f03-9832-341134ffcb75" />


