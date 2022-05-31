# An Analysis of Kickstarter Campaigns

## Overview of Project
Kickstarter campaigns were compared to evaluate outcomes for plays based on launch dates and fundraising goals.

### Purpose
The purpose is to uncover trends in the available data to better inform the success of Louise's campaign to crowdfund her play entitled *Fever*.  
Her anticipated budget starts at $10000.

## Analysis and Challenges
The analysis was completed in Microsoft Excel by creating PivotTables and PivotCharts.

In order to look at theater outcomes by launch date, the launch date was converted from Unix time to a readable format using an online conversion tool and the year was isolated from the launch date using the YEAR function. 
The Parent and Subcategory data column was split in order to filter on only successful, failed and canceled Theater campaigns. 
The following chart "Theater Outcomes Based on Launch Date" is showing outcomes for completed campaigns from 2009-2016.
To create this chart a PivotTable and PivotChart were built, filtering on Parent Category and Years.  
![Theater Outcomes vs Launch](/resources/Theater_Outcomes_vs_Launch.png)
The x-axis represents the launch month and the y-axis represents the number of campaign outcomes. 

To evaluate trends in campaign outcomes based pledge goals, a new table was created which used the COUNTIFS function to count the number of outcomes at a particular fundraising goal interval.
The following chart "Campaign Outcomes Based on Goals" is showing the percentage of each outcome level at each financial goal interval.
![Outcomes vs Goals](/resources/Outcomes_vs_Goals.png)
The x-axis shows each financial goal interval and the y-axis shows the percentage of campaign outcomes.

### Analysis of Outcomes Based on Launch Date
May to July had the largest number of successful theater launches and also the largest overall number of campaign launches.
During this timeframe, the number of failed launches remained fairly constant, within 2 outcomes of 50 failures per month.
Campaigns launched in December were overall low, with nearly equivalent outcomes for successes and failures.
Cancelled campaigns were overall few and do not appear to change relative to launch date.

### Analysis of Outcomes Based on Goals
Successful campaigns exceeded failed campaigns at overall goal intervals:
- $14999 and less, with the largest success rate over failures at goals $4999 and less
- between $35000 and $44999

There was a large percentage of failures between $25000 and $34999.
Above $45000, nearly all campaigns failed with a few exceptions greater than $50000.

### Challenges and Difficulties Encountered
It is important to be mindful of maintaining the integrity and accuracy of the whole dataset when working in the spreadsheet.
For example, awareness of filtering and clearing filters is important. If additional columns are added to a filtered dataset and autofilled using the Fill Handle, it will create blanks for the entries which have been filtered out.
Any error introduced could potentially be compounded upon by building out columns which use functions to look at other columns in the dataset.
Functions should be carefully inspected to ensure the correct columns or cells are referenced.  
If these kinds of compounded errors are go unnoticed, the analysis will likely be skewed or invalid.
It is also a good idea to backup the file at different timepoints to make sure that if an error is uncovered, the analysis can be picked up from a previous timepoint without having to start completely over.

## Results

1. What are two conclusions you can draw about the Outcomes based on Launch Date?

Launching a kickstarter campaign in May or June may increase the success of achieving the fundraising goal.
After October the number of successful campaign drops and it is at the lowest in December.

2. What can you conclude about the Outcomes based on Goals?

Louise may improve her likelihood of success if she keeps her budget under $4999.  
There is a slightly higher percentage of successful outcomes at her anticipated budget which starts at $10000, but the percentage of failures is very close in that goal interval.

3. What are some limitations of this dataset?

This dataset is more than 5 years old.  
There are not nearly as many data points for plays outcomes with fundraising goals more than $10000.
The confidence level for making inferences above this funraising goal is lower.

4. What are some other possible tables and/or graphs that we could create?

Percentage of Theather Outcomes Based on Launch Date would help show successes as a function of total outcomes.
This could also be filtered down from the parent category to only look at plays.




