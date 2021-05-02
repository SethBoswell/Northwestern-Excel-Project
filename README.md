# An Analysis of Kickstarter Campaigns
This project provides summary statistics and visualizations to analyze significant trends in Louise's Kickstarter dataset.

## Overview of Project
Louise's dataset contains 4114 individual "kickstarter" fundraising campaigns spread across 21 different countries. For each campaign, there is data on its launch date, end date, goal or target fundraising amount, amount pledged by backers, number of backers, and category/subcategory. Louise wanted me to provide a breakdown of how theater campaigns and plays performed in her dataset. Specifically, she wanted to know how theater campaigns performed over time based on their outcome (successful, failed, or canceled) and how plays performed based on their set goal amount. 

For my analysis, I created pivot tables and charts/visualizations to provide answers to Louise's questions. I will go into further detail on my analysis in the below section

## Theater Outcomes by Launch Date

### Analysis and Challenges
Louise wanted to understand how theater campaigns in her Kickstarter dataset performed over time. To help her with this, I created a pivot table from the original dataset. You are able to filter by Parent Category, which is currently set as "theater" since Louise wanted to know about theater campaigns, and the year the campaign was launched, which currently is unfiltered (so all years are included in the summary statistics). The pivot table provides a monthly breakdown of the the number of theater campaigns that were either successful (i.e., fundraising met goal amount), failed, or canceled. For example, there were a total of 56 campaigns that were started in a January between 2009 and 2017 (the year ranges of the dataset). There were also 96 total campaigns that were launched in January and a total of 839 campaigns that were successful. The full pivot table statistics are included below.

![Theater Outcomes by Launch Date Count Pivot Table](https://github.com/SethBoswell/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch%20Pivot%20Table.png)

To identify monthly trends in the dataset, I created a line chart from the pivot table statistics that graphs the number of successful, failed, and canceled campaigns across each month. This chart is included below as well. 

![Theater Outcomes by Launch Date Count Line Chart](https://github.com/SethBoswell/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png)

I provided a further breakdown of the datset by creating an additonal pivot table that calculates, for each month, the percent of camapaigns that were successful, failed, and canceled. These statistics were also placed in a line chart. Included below is an image of the pivot table data and line chart.  
![Theater Outcomes by Launch Date Percents Pivot Table](https://github.com/SethBoswell/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch%20Percents%20Pivot%20Table.png)

![Theater Outcomes by Launch Percents Line Chart](https://github.com/SethBoswell/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch%20Percents%20Chart.png)

I thought the most challenging portion of this part was creating the second pivot table, which calculates the proportion of campaigns that were successful vs cancelled vs failed for each month. I had to figure out how to show values as "% of row total" from the pivot table options in order to display the data how I wanted. I thought this created a nice pivot table that details whether there were certain months that saw a significant decrease in the proportion of campaigns that were successful. 
### Results
You can see from the first pivot table and line graph above that number of successful theater campaigns peaked heavily in May and then steadily declined from there. By December, the number of successful campaigns is almost equal to the number of failed ones. A possible explanation is that theaters become increasingly popular in the summer months as people tend to spend more on entertainment and enjoyable activities, so they receive more funding. In the winter months, Louise's targeting goals may be too high since  less campaigns are reaching their goal targets. However, further analysis would be necessary to determine this fact. You can also tell that the number of failed campaigns remained relatively consistent across time and there were only a few campaigns each month that ended up being canceled. 

Furthermore, based on the second pivot table and line graph above, you can see that the proportion of campaigns that are successful, failed, or canceled remains relatively stable across the months, except in December. There is an uptick in the proprotion of campagins that fail and a downtick in the proprtion that succeed in this month. Based on these facts, I would recommend revising goal targets downward in December to have more campaigns meet their goals. Another option would be to increase funding for promotional activities during this month to increase funding and increase the amount and proportion of campaigns that succeed. 


## Outcomes based on Goals

### Analysis and Challenges
Louise also wanted to know the number and proportion of *plays* that were successful for different goal amounts. To accomplish this task, I broke up the goal amounts into the following buckets:
- Less than 1000
- 1000 to 4999
- 5000 to 9999
- ...
- Greater than 50000

For each of these buckets, I calculated the number of plays that were successful, failed, or canceled. I then calculated the total number of plays for each bucket and the proportion that were successful vs failed vs canceled. You can see the results of this analysis below.

![Outcomes Based on Goals Table](https://github.com/SethBoswell/kickstarter-analysis/blob/main/Outcomes_vs_Goals%20Table.png)

I then created a line graph that graphs the proportion of successful, failed, and canceled plays for each goal bucket. You can see the results of that analysis below.

![Outcomes Based on Goals Line Chart](https://github.com/SethBoswell/kickstarter-analysis/blob/main/Outcomes_vs_Goals.png)

The most challenging aspect of this part of the project was creating the 'CountIfs' formulas to account for all of the different buckets. I had to ensure that all my CountIf formulas were properly separating out the goal amounts into each bucket, which included making sure that I was dealing with "fringe" cases by using the ">=" and "<=" sign.

### Results
One interesting observation was that there were 0 cancelled plays across all of the different goal amount buckets. I am not sure why this is the case; however, it could be interesting to do further analysis to compare plays to other Theater campaign subcategories such as "musicals" and "spaces" (see Limitations and Future Work).

The table above shows that the majority of the plays had goal amounts less than about $25,000. The line chart indicates that plays with goal amounts less than about $15,00 tend to have a higher proportion that are successful instead of failing. The data is mixed for plays with goal amounts from about $15,000 to $45,000 and, for plays greater than $45,000, there is a higher proportion that fail then are successful. I would recommend that Louise continue to focus on plays with smaller goal amounts to increase the amount of plays that end up successful. She could also revise her goal amounts downward for plays costing more than $45,000 since these plays are less likely to raise this amount. 

## Limitations and Future Work

