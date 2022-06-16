# Kickstarter Campaign Analysis

## Overview of Project

### Purpose

Louise is an up and coming playwright and she wants to start a crowdfunding campaign to fund her play, Fever. She has asked for help in analyzing data from previous and ongoing Kickstarter campaigns in order to help her own campaign be successful. The purpose of this project was to look for specific factors that make a campaign successful and use those insights to help Louise plan her own campaign.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

This chart shows the outcomes of theater campaigns based on the launch date. I first converted the launch date from a Unix timestamp to a standard format using the date formula, then made a PivotTable using the outcomes, parent category, and the newly converted launch date. After filtering the category to only theater campaigns, I counted the number of each outcome per month.

![Unix_Timestamp_Conversion](https://user-images.githubusercontent.com/106830513/174194183-a59bb67d-7343-440f-b4cd-86b1d7d9853d.png)
![Theater_Outcomes_Table](https://user-images.githubusercontent.com/106830513/174193584-977b49de-4094-41d0-b90a-50b7c0a40ab7.png)

### Analysis of Outcomes Based on Goals

This chart shows the outcomes of play campaigns based on their monetary goal. Using the COUNTIFS function, I determined goal ranges and counted the number of each outcome that fell within each goal range for each campaign with the subcategory of plays. Next, I added up all of the projects to get the total projects for each goal range and created percentages based on the outcomes within each goal range. Then, I created a line chart depicting these percentages for each outcome within each goal range.

![COUNTIFS_function](https://user-images.githubusercontent.com/106830513/174193627-41189438-92d7-434a-a223-36ae190990b5.png)

### Challenges and Difficulties Encountered

One difficulty I faced was with the COUNTIFS function. I had never used it before. I used the option within Excel for "Help on this function" which took me to a Microsoft support site (https://support.microsoft.com/en-us/office/countifs-function-dda3dc6e-f74e-4aee-88bc-aa8c2a866842?ui=en-us&rs=en-us&ad=us). After reading through it and watching the video, I was ready to try it within my file and it worked!

## Results

### What are two conclusions you can draw about the Outcomes based on Launch Date?

One conclusion for the Outcomes based on Launch Date is that the summer months seem to be the best time to launch a campaign, from April through August, with May, June, and July historically being the most successful months. A second conclusion is that most campaigns are also being launched during these summer months, so the data may be skewed unless a percentage is included.

### What can you conclude about the Outcomes based on Goals?

A conclusion for the Outcomes based on Goals is that there is a higher chance of success with a lower goal, roughly less than $15,000.

### What are some limitations of this dataset?

A limitation of this dataset is that this data spans many years, ranging from 2009 to 2017. I would be more interested in only the most recent few years of data, maybe three to five years max, as that would be most representable of what Louise's campaign may experience today.

### What are some other possible tables and/or graphs that we could create?

I would recommend creating two additional charts: one showing the correlation between the number of backers and the outcome and another showing the correlation between the average donation and the outcome. This may help Louise determine if she should market her campaign to get a lot of backers donating small amounts or shoot for less backers donating large sums.
