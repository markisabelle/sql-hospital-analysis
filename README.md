# Hospital Analytics Project

A SQL-based analysis of hospital patient records to assess operational efficiency, identify cost drivers, and understand patient behavior patterns.

## Project Overview

This project analyzes 75,500+ multi-year hospital patient records using MySQL to provide data-driven insights that could help hospitals reduce readmissions and improve cost efficiency. The analysis focuses on three key areas: encounter patterns, cost and coverage insights, and patient behavior.

## Dataset

- **Source**: Hospital encounter records (MySQL database)
- **Size**: 75,500+ records
- **Key Tables**: `encounters`, `procedures`
- **Time Period**: Multi-year data

## Analysis Objectives

### 1. Encounters Overview
- **Total encounters by year**: Tracked encounter volume trends over time
- **Encounter class distribution**: Analyzed the percentage breakdown of ambulatory, outpatient, wellness, urgent care, emergency, and inpatient visits
- **Encounter duration**: Calculated what percentage of encounters lasted over vs. under 24 hours

### 2. Cost & Coverage Insights
- **Uninsured encounters**: Identified that 48.7% of encounters (13,586 records) had zero payer coverage
- **High-frequency procedures**: Determined the top 10 most common procedures and their average base costs
- **High-cost procedures**: Found the top 10 procedures with the highest average base costs
- **Payer analysis**: Calculated average total claim costs broken down by insurance payer

### 3. Patient Behavior Analysis
- **Patient admission trends**: Tracked unique patient admissions quarterly over time
- **30-day readmissions**: Identified 772 patients readmitted within 30 days of a previous encounter
- **Frequent readmissions**: Analyzed which patients had the most readmissions

## Key Findings

- **48.7% of encounters** had zero payer coverage, representing a significant uninsured patient population
- **772 patients** were readmitted within 30 days, indicating opportunities for improved post-discharge care
- High-frequency procedures and high-cost procedures were identified to help prioritize operational improvements

## Technical Skills Demonstrated

- Complex SQL queries with window functions (LAG, PARTITION BY)
- Common Table Expressions (CTEs) for multi-step analysis
- Date functions and time-based calculations (TIMESTAMPDIFF, DATEDIFF, QUARTER)
- Conditional aggregation using CASE statements
- Data grouping and percentage calculations

## Business Impact

These insights could help hospitals:
- Reduce readmissions by 10-15% through targeted post-discharge interventions
- Improve payer cost efficiency by understanding coverage patterns
- Optimize resource allocation based on encounter class trends
- Better manage high-cost procedures and associated costs

## Tools & Technologies

- **Database**: MySQL
- **Language**: SQL
- **Key Techniques**: Window functions, CTEs, date calculations, conditional aggregation

## Repository Structure

```
hospital_analytics/
├── README.md
└── hospital_analysis.sql
```

## How to Use

1. Connect to a MySQL database with the hospital dataset
2. Run the SQL queries in `hospital_analysis.sql`
3. Review the results for operational insights

## Author

Mark Isabelle  
[LinkedIn](https://linkedin.com/in/mark-isabelle-a113b8325) | [GitHub](https://github.com/markisabelle)
