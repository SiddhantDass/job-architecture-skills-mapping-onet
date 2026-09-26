# Job Architecture & Skills Mapping (O*NET)

## Business Problem
An HR Operations or Talent Acquisition analyst needs to compare skill
requirements across HR and adjacent occupations to identify role
consolidation opportunities and internal mobility paths.

## Data Source
- O*NET Database, published by the U.S. Department of Labor
  (Employment and Training Administration)
- Source: https://www.onetcenter.org/database.html
- Files used: Occupation Data, Essential Skills, Job Zones
- Licence: Creative Commons (CC BY 4.0)

## Scope
14 occupations across three groups: Core HR/People roles, HR Operations/
Administration roles, and Adjacent People/Business Operations roles.
One occupation ("Business Operations Specialists, All Other") was
excluded — O*NET does not publish Essential Skills ratings for this
"All Other" residual category.

## What This Data Can and Cannot Show
This data shows national reference skill-importance ratings for each
occupation, on a 0-5 scale. It cannot tell you what a specific employer's
version of a role actually requires, and it does not predict who will
succeed in a role — it is a general taxonomy, not a company-specific
job evaluation.

## Method
1. Filtered O*NET Essential Skills data to the Importance (IM) scale
2. Scoped to 15 HR and adjacent occupations, later reduced to 14
3. Built a skill-importance matrix and bar chart in Power BI
4. Added slicers for Job Zone and Scope Group

## Tools Used
Excel (data cleaning, XLOOKUP, pivot tables), Power BI (data modeling, DAX, visuals)

## Dashboard Preview
![Dashboard screenshot](screenshotsdashboard-overview.png)

## Files in This Repo
- `onet_clean_for_powerbi.xlsx` — cleaned data workbook
- `Job_Architecture_Dashboard.pbix` — Power BI dashboard file
- `screenshots/` — dashboard preview images

## How to Reproduce
1. Download the Essential Skills, Occupation Data, and Job Zone files
   from onetcenter.org/database.html
2. Follow the cleaning steps described above in Excel
3. Load the cleaned tables into Power BI and relate them on O*NET-SOC Code
