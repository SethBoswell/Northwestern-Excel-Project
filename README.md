# An Analysis of Kickstarter Campaigns
This project provides summary statistics and visualizations to analyze significant trends in Louise's Kickstarter dataset.

## Overview of Project
Louise's dataset contains 4114 individual "kickstarter" fundraising campaigns spread across 21 different countries. For each campaign, there is data on its launch date, end date, goal or target fundraising amount, amount pledged by backers, number of backers, and category/subcategory. Louise wanted me to provide a breakdown of how theater campaigns and plays performed in her dataset. Specifically, she wanted to know how theater campaigns performed over time based on their outcome (successful, failed, or canceled) and how plays performed based on their set goal amount. 

For my analysis, I created pivot tables and charts/visualizations to provide answers to Louise's questions. I will go into further detail on my analysis in the below section

## Theater Outcomes by Launch Date

### Analysis and Challenges
Louise wanted to understand how theater campaigns in her Kickstarter dataset performed over time. To help her with this, I created a pivot table from the original dataset. You are able to filter by Parent Category, which is currently set as "theater" since Louise wanted to know about theater campaigns, and the year the campaign was launched, which currently is unfiltered (so all years are included in the summary statistics). The pivot table provides a monthly breakdown of the the number of theater campaigns that were either successful (i.e., fundraising met goal amount), failed, or canceled. For example, there were a total of 56 campaigns that were started in a January between 2009 and 2017 (the year ranges of the dataset). There were also 96 total campaigns that were launched in January and a total of 839 campaigns that were successful. The full pivot table statistics are included below.

![Theater Outcomes by Launch Date Count Pivot Table](https://github.com/SethBoswell/kickstarter-analysis/blob/main/Outcomes_vs_Goals%20Pivot%20Table.png)

To identify monthly trends in the dataset, I created a line chart from the pivot table statistics that graphs the number of successful, failed, and canceled campaigns across each month. This chart is included below as well. 

![Theater Outcomes by Launch Date Count Line Chart](https://github.com/SethBoswell/kickstarter-analysis/blob/main/Outcomes_vs_Goals%20Pivot%20Table.png)

I provided a further breakdown of the datset by creating an additonal pivot table that calculates, for each month, the percent of camapaigns that were successful, failed, and canceled. These statistics were also placed in a line chart. Included below is an image of the pivot table data and line chart.  
![Theater Outcomes by Launch Date Percents Pivot Table](https://github.com/SethBoswell/kickstarter-analysis/blob/main/Outcomes_vs_Goals%20Percents%20Pivot%20Table.png)

![Theater Outcomes by Launch Percents Line Chart](https://github.com/SethBoswell/kickstarter-analysis/blob/main/Outcomes_vs_Goals%20Percents%20Chart.png)
### Results
You can see from the first pivot table and line graph above that number of successful theater campaigns peaked heavily in May and then steadily declined from there. By December, the number of successful campaigns is almost equal to the number of failed ones. A possible explanation is that theaters become increasingly popular in the summer months as people tend to spend more on entertainment and enjoyable activities, so they receive more funding. In the winter months, Louise's targeting goals may be too high since  less campaigns are reaching their goal targets. However, further analysis would be necessary to determine this fact. You can also tell that the number of failed campaigns remained relatively consistent across time and there were only a few campaigns each month that ended up being canceled. 

Furthermore, based on the second pivot table and line graph above, you can see that the proportion of campaigns that are successful, failed, or canceled remains relatively stable across the months, except in December. There is an uptick in the proprotion of campagins that fail and a downtick in the proprtion that succeed in this month. Based on these facts, I would recommend revising goal targets downward in December to have more campaigns meet their goals. Another option would be to increase funding for promotional activities during this month to increase funding and increase the amount and proportion of campaigns that succeed. 


