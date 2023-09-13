# Road Accident Dashboard Project

## Project Overview

Clients want to create a Road Accident Dashboard for Year 2021 and 2022 to gain insights into road accidents and casualties. The dashboard will address the following requirements:

## Primary KPIs

1. **Total Casualties and Total Accidents for Current Year and YOY Growth**
   - Calculate the total casualties and total accidents for the current year.
   - Calculate Year-over-Year (YOY) growth percentages for both casualties and accidents.

2. **Total Casualties by Accident Severity for Current Year and YOY Growth**
   - Analyze total casualties categorized by accident severity for the current year.
   - Calculate YOY growth percentages for each accident severity category.

## Secondary KPIs

3. **Total Casualties with Respect to Vehicle Type for Current Year**
   - Break down total casualties based on vehicle types for the current year.

4. **Monthly Trend**
   - Display a trend analysis showing the compression of casualties for the current year compared to the previous year on a monthly basis.

5. **Casualties by Road Type for Current Year**
   - Analyze casualties based on different road types for the current year.

6. **Current Year Casualties by Area**
   - Segment casualties based on different geographic areas for the current year.

7. **Current Year Casualties by Location**
   - Segment casualties based on specific locations for the current year.

8. **Current Year Casualties by Day/Night**
   - Categorize casualties as day and night for the current year.

9. **Total Accident and Total Casualties by Location**
   - Calculate the total number of accidents and casualties by location.

## Implementation

   - After cleaning data first create a new table Calender which will contain columns such as date , month , year and connect it with main column
   - then create another table named Measure which will we use to store different measures for calculation \
   - Curr Year Casulities = TOTALYTD(sum(Table1[Number_of_Casualties]),calender[Date])
   - Past Year Casulities = CALCULATE(sum(Table1[Number_of_Casualties]),SAMEPERIODLASTYEAR(calender[Date]))
   - YOY Casualties = ([Curr Year Casulities]-[Past Year Casulities])/[Past Year Casulities]
   - similar steps with the accident column
   - Then draw different visuals 

## Data Sources

The dashboard will utilize data sources related to road accidents and casualties for the years 2021 and 2022.

## Usage

The dashboard will provide a user-friendly interface for clients to explore and analyze road accident data, facilitating data-driven decision-making.

