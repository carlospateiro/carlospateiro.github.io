# Divvy: Customer Usage Analysis

**Project description:** This project dives into the data to understand how Casual and Member customers utilize Divvy bike-sharing services in Chicago, shedding light on key usage patterns and behaviors to inform strategic decisions and service improvements.

This report will follow the structure proposed in the **Google Data Analytics Certificate:**

* **Ask:** Business Challenge/Objective/Question
* **Prepare:** Data generation, collection, storage, and data management
* **Process:** Data cleaning/data integrity
* **Analyze:** Data exploration, visualization, and analysis
* **Share:** Communicating and interpreting results
* **Act:** Putting your insights to work to solve the problem.

## 1. ASK

### Guiding questions:
* How does the usage of Divvy bikes differ between annual members and casual riders?

## 2. PREPARE
### Key tasks

* Download data and store it appropriately.
* Identify how it’s organized.
* Sort and filter the data.
  
### Step 1: Load Packages

### Step 2. Concatenating all the CSVs files into one data frame.

## 3. PROCESS
### Key tasks

* Check the data for errors.
* Choose your tools.
* Transform the data so you can work with it effectively.
* Document the cleaning process.
  
### DATA CLEANING

### Step 3. Removing any duplicate rows.

<img src="C:\Users\Carlos\OneDrive\Pictures/Frame2.jpg?raw=true"/>

### Step 4. Parsing date time columns.
### Step 5. Calculating ride duration

As we can see from the above information, there are negative values. Having into account that this is not possible, we will need to follow these steps:

* Investigate the data and identify the source of the negatives values. Perhaps there is a glitch in the software or hardware that records the rides.
* Perform data cleaning to ensure the analysis is based on accurate and consistent data.
* Lastly, it would be advisable to reach out to stakeholder and ask for clarification in order to avoid any misinterpretation.

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Step 6. Checking how many rides there are with negative value
### Step 7. Removing rows where the column ride_duration has negative value.

## DATA MANIPULATION
### Step 8. Creating new columns with the starting month, day, and hour.
This will help us to easily detect if there are any seasonal, weekly, or daily trends in the riding behavior.
### Step 9. Transforming the columns “member_casual” and “rideable_type” data type to factor.

## 4. ANALYZE
### Key tasks
* Aggregate your data so it’s useful and accessible.
* Organize and format your data.
* Perform calculations.
* Identify trends and relationships.
* This function will help us to maintain the same width and height of all plots.

**Chart 01 - Casual vs members distribution**
As an initial step in the analysis phase, we would like to determine the proportion of data corresponding to member and casual riders.

According to the data presented in Chart 01, members constitute a larger proportion of the dataset at 59.67%, which is 19% higher than that of casual riders.

**Chart 02 - Average trip duration: Members vs casual**

Although members utilized the service 19% more frequently, data indicates that casual riders tend to engage in longer rides. This suggests that casual riders may use the service for recreational purposes. However, further analysis is required to draw more definitive conclusions.

**Chart 03 - Total rides taken: Rider type vs month**

The data reveals a considerable increase in bicycle usage during the warmer months of the year, particularly from May through September.

In July, casual ridership peaked at 406,013 rides, accounting for 17.48% of total usage. Meanwhile, member ridership reached its highest point in August with 426,969 rides or 12.76% of total usage.

**Chart 04 - Total rides taken: Rider type vs day of the week**

Analysis of Chart 04 reveals the following key insights:

* Saturday has the highest number of rides.
* Casual riders show a significant increase in usage during weekends.
* Member usage is considerably higher from Monday to Friday.

**Chart 05 - Total rides taken: Rider type vs hour of the day**

The data reveals differences in usage patterns between members and casual riders. Members exhibit an early peak in usage from 6 to 8 AM, with a subsequent decline beginning at 9 AM. In contrast, casual riders demonstrate a gradual increase in usage from 6 AM to 5 PM.

**Chart 06 - Distribution by hour of the day divided by day of the week (Facet Wrap)**

Chart 06 reveals a couple of key insights:

* There is a clear difference in usage patterns between weekdays and weekends.
* The usage patterns of member riders suggest that the service is primarily utilized for commuting purposes from Monday to Friday.
* During weekends, usage peaks in the afternoon, increasing progressively from 8 AM and reaching its maximum at 3 PM before starting to decline.

**Chart 07 - Distribution by hour of the day in the weekend**

The chart below help us to better understand the riding patterns of both members and casual riders during weekends.

**Chart 08 - Distribution by hour of the day in the midweek**

The chart below provides information of riding patterns from Monday to Friday. A notable difference can be noted when compared to the data presented in Chart 7.

**Chart 09 – Distribution of type of bikes**

As we can see, electric bikes are the most popular option among riders, followed by classic bikes and docked bikes. However, the noticeably low usage of docked bikes suggests that there may be an issue with the data.

**Chart 10 - Rideable type distribution: Members vs casual**

The data reveals that docked bikes were not made available to members. This information help us to understand the discrepancy in the usage of these bikes observed in chart 09.

Apart from this, we can observe the following:

* Classic bikes were the go-to choice among members riders.
* Electric bikes were preferred by casual riders.

## 5. SHARE
### Key tasks

1. Determine the best way to share your findings.

In a typical work environment, it would be ideal to share our findings through a presentation to all stakeholders. However, in this particular situation, all relevant information was effectively communicated using the tools available on this platform.

2. Create effective data visualizations.

The visualizations presented in this analysis are both effective and easy for viewers to understand the data and insights being conveyed.

3. Present your findings.

Based on the analysis, it can be concluded that there are notable differences between member and casual riders in terms of their usage of the bike sharing service:

Members constitute a larger proportion of the dataset and utilize the service more frequently.
Casual riders tend to engage in longer rides, suggesting recreational use.
Bike usage increases during the warmer months, particularly from May through September.
Saturday has the highest number of rides, with casual riders showing a significant increase in usage during weekends and member usage being considerably higher from Monday to Friday.
Members exhibit an early peak in usage from 6 to 8 AM, with a subsequent decline beginning at 9 AM, while casual riders demonstrate a gradual increase in usage from 6 AM to 5 PM.
Electric bikes are the most popular option among riders, followed by classic bikes and docked bikes.
4. Ensure your work is accessible.

The information in this notebook is presented in a clear and organized manner, making it easily accessible to readers.

## 6. ACT
### Guiding questions
1 - What is your final conclusion based on your analysis?

The analysis of Cyclistic data suggests that the service is mainly utilized for commuting purposes by members, while casual riders tend to use it for recreational purposes. The higher usage of electric bikes and classic bikes also implies a preference for convenient and easy-to-use options. The data further highlights the importance of seasonality and weekends in bike usage patterns, which should be taken into account when designing marketing campaigns and service improvements.

2 - How could your team and business apply your insights?

This analysis has provided valuable insights regarding the usage patterns of both members and casual riders. As such, this information should be used not only to create marketing campaigns aimed at increasing annual memberships, but also to improve the overall quality of the service.

3 - What next steps would you or your stakeholders take based on your findings?

Based on the data presented, it would be advisable to take action and create marketing campaigns to achieve the business goals.

4 - Is there additional data you could use to expand on your findings?

Obtaining demographic data to analyze the riding patterns of both members and casual riders would be valuable. This data could help to target future marketing campaigns.

