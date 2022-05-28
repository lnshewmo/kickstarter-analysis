# kickstarter-analysis
Kickstarter Data Analysis - Uncover Trends
# An Analysis of Kickstarter Campaigns

## Overview of Project
Kickstarter campaigns for plays were compared to evaluate outcomes based on launch dates and fundraising goals.

### Purpose
The purpose is to uncover trends in the available data to better inform the success of Louise's campaign to crowdfund her play entitled *Fever*.

## Analysis and Challenges

The analysis was completed in Microsoft Excel by creating PivotTables and PivotCharts.

In order to look at theater outcomes by launch date, the launch date was converted from Unix time to a readable format using an online conversion tool and the year was isolated from the launch date using the =YEAR( function. 
The Parent and Subcategory data column was split in order to filter on only successful, failed and canceled Theater campaigns. 
The following chart "Theater Outcomes Based on Launch Date" is showing outcomes for completed campaigns from 2009-2016.
To create this chart a PivotTable and PivotChart were built, filtering on Parent Category and Years.  
![Theater Outcomes vs Launch](/Theater_Outcomes_vs_Launch.png)
The x-axis represents the month of the launch and the y-axis represents the number of launches. 

To evaluate trends in campaign outcomes based pledge goals, a new table was created which used the =COUNTIFS( function to count the number of outcomes at a particular fundraising goal interval.
The following chart "Campaign Outcomes Based on Goals" is showing the percentage of each outcome level at each financial goal interval.
![Outcomes vs Goals](/Outcomes_vs_Goals.png)
The x-axis shows each goal interval and the y-axis shows the percentage of outcomes.

### Analysis of Outcomes Based on Launch Date

### Analysis of Outcomes Based on Goals

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
