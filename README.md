# Cyclistic Bike-Share Analysis Case Study
By Jose Angel Gonzalez

## Business Task
### Objective:
- The goal is to understand how Cyclistic's annual members and casual riders use bikes differently. Insights from this analyusis will inform a marketing strategy aimed at converting casual riders into annual members.

### Key Questions:
1. How do annual members and casual riders use cyclistic bikes differently?
2. Why would casual riders buy Cyclistic annual memberships?
3. How can Cyclistic use digital media to influence casual riders to become members?

## Data Sources
### Description:
- The data used in this analysis comes from Cyclistic's historical bike trip data. This dataset includes fields such as trip duration, start time, end time, start station name, end station name, user type, and more. 			        		

## Data Cleaning and Preparation
- BigQuery was used for all data cleaning and preparation tasks
### Steps:
#### 1. Data Import:
- The dataset was imported 
#### 2. Filtering:
- Trips with null values in critical fileds like 'end station name' were filtered out to ensure data integrity. [View Query](https://github.com/Grandpa-3/cyclistic_prework/blob/main/Cyclistic.sql)

#### 3. Date Parsing:
- a calculated field was created to extract the day of the week from the 'start time', facilitating the analysis of weekly ride patterns.
#### 4. Outlier Removal:
- Trips with a duration exceeding 24 hours were identified as outliers and excluded to maintain a realistic view of ride behaviors.
#### 5. User Type Classification:
- Data was segmented into 'Casual Riders' and 'Members' based on the 'user type' field for comparative analysis.
#### ![Execution Graph](https://github.com/Grandpa-3/Cyclistic/blob/main/ExecutionGraph.png?raw=true)


## Analysis Summary
### Key Findings:

**Ride Duration:**
- Casual riders tend to have longer ride durations compared to annual members, indicating that casual riders might use bikes more for leisure rather than communting.
#### ![Execution Graph](https://github.com/Grandpa-3/Cyclistic/blob/401916d6feddfd60cf90ba3a868f119e50368b8b/RideDuration_UsageDaily.png)

**Usage by Day of the Week:**
- Annual members show consistent usage througout the workweek, while casual riders predominantly use bikes on weekends, sugesting a leisure-oriented pattern.

**Station Usage:**
- Casual riders frequently start and en teir trips at stations near tourist attractions and parks, while annual members are more likely to use stations near business districts and residential areas.
#### ![Station Usage](https://github.com/Grandpa-3/Cyclistic/blob/43daf19bdf43f79e8639bd8efaf433a1fedf8bda/StationUsage.png)

### [Click to see Cyclistic Dashboard](https://public.tableau.com/app/profile/jose.gonzalez.ramirez/viz/Cyclistic_17262131192190/CyclisticNY)

## Conclusion
  - The analysis provides a clear understanding of how casual riders and annual members differ in their usage of Cyclistic's bike-share service. By targeting specific user behaviors and preferences, Cyclistic can effectively convert more casual riders into loyal annual members, ensureing sustained growth and profitability.

## Recommendatons:

### Based on the analysis, the following strategies are recommended:
#### 1. Targeted Marketing Campaigns:
- Develop campaings focused on converting casual riders into members by emphasizing the benefits of memebership for frequent users, particularly for commuting.
#### 2. Weekend Membership Iniciatives:
- Offer special incentives or discounts on annual memberships for users who frequently ride on weekends, encouraging them to consider membership for more regular use.
#### 3. Leverage Digital Media:
- use digital media channels to highlight membership advantages, such as cost savings and convenience, to casual riders, especially targeting areas around tourist attractions where casual ridership is high.

## [Go back to my Webpage](https://JoseAGonzalezR.github.io/Jose_AGonzalez.github.io/)
