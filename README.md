# Project 1 - McGill Admission Profile Overview

## Overview
This project is designed to show an overview of admission profile (student distribution) of McGill University through 2015-2021. 

The programming used to compelete the project is Python.

Data is scraped from: [McGill Admission Profile](https://www.mcgill.ca/es/admissions-profile) 
(`Entering class by region **` and `Undergraduate entering class by admissions unit`) using Beautifulsoup package.

Data are cleaned, analyzed and visualized with the application of numpy, Pandas, seaborn and matlibplot.

## Main Table Summary
The two main tables used in analysis and visualization are exported after data scraping with a absolute path due to an error raised when a relative path was used. 
Viewers/users will need to change the path (in step 1 and 2) or replace all the occurance of `field` to `by_field` and `region` to `by_region` (in Step 2)

### `by_field_1` - cleaned pd.dataframe from `field` or `by_field`(98 rows * 5 columns, 0 Null)
Columns:

0. Undergrade(o): Field of study
1. Applicants(int64): Count of applicants
2. Registered Students(int64): Count of registered students
3. Year(int64): Year as number              
4. Year_cat(o): Year as category

### `by_region_1` - cleaned pd.dataframe from `region` or `by_region` (42 rows * 9 columns, 0 Null)
Columns:

0. Region(o): Canada, Overseas, -Not Reported, Quebec, Total, USA
1. Undergrade(float64): Count of undergrade students
2. Undergrade Rate(float64): Percentage of undergrades in total
3. Continuing Education(int64): Count of continuing education students
4. Continueing Ed Rate(float64): Percentage of continuing education in total
5. Graduate(float64): Count of graduate students
6. Graduate Rate(float64): Percentage of graduate in total
7. Year(int64): Year as number
8. Year_cat(o): Year as category

## Questions to Answer
### By field
1. Student distribution by study field - bar chart and pie chart
2. Applicants and registered student number change by year - line chart
3. Top 3 field that are most difficult to get in - bar chart

### By region
1. Undergraduate student distribution by region - line chart
2. Student distribution by region among all three study levels - pie chart

