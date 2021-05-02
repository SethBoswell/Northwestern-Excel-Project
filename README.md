# An Analysis of Kickstarter Campaigns
This project provides summary statistics and visualizations to analyze significant trends in Louise's Kickstarter dataset.

## Overview of Project
Louise's dataset contains 4114 individual "kickstarter" fundraising campaigns spread across 21 different countries. For each campaign, there is data on its launch date, end date, goal fundraising amount, amount pledged, number of backers, and category/subcategory. Louise wanted me to provide a breakdown of how theater campaigns and plays performed in her dataset. Specifically, she wanted to know how theater campaigns performed over time based on their outcome (successful, failed, or canceled) and how plays performed based on their set goal amount. 

For my analysis, I created pivot tables and charts/visualizations to provide answers to Louise's questions. I will go into further detail on my analysis in the below section

##Theater Outcomes by Launch Date

###Analysis and Challenges
Louise wanted to understand how theater campaigns in her Kickstarter dataset performed over time. To help her with this, I created a pivot table from the original dataset. You are able to filter by Parent Category, which is currently set as "theater" since Louise wanted to know about theater campaigns, and the year the campaign was launched, which currently is unfiltered (so all years are included in the summary statistics). The pivot table provides a monthly breakdown of the the number of theater campaigns that were either successful (i.e., fundraising met goal amount), failed, or canceled. For example, there were a total of 56 campaigns that were started in a January between 2009 and 2017 (the year ranges of the dataset). There were also 96 total campaigns that were launched in January and a total of 839 campaigns that were successful. The full pivot table statistics are included below.

![Outcome by Launch Date Pivot Table](C:\Users\seths\OneDrive\Documents\Northwestern Data Science Bootcamp\Classwork\Module 1\Module 1 Challenge Assessment\Resources\Outcomes_vs_Goals Pivot Table.png)

To identify monthly trends in the dataset, I created a line chart from the pivot table statistics that graphs the number of successful, failed, and canceled campaigns across each month. This chart is included below as well. 



###Results
You can see from the pivot table data and line graph above that number of successful theater campaigns peaked heavily in May and then steadily declined from there. A possible explanation is f
