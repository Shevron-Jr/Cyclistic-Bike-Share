## Cyclistic-Bike-Share
#### Capstone Project

Link to Cyclistic Trip Data: [here](https://divvy-tripdata.s3.amazonaws.com/index.html)

## BUSINESS TASK:
### What is the problem?

1.How do annual members and casual riders use Cyclistic bikes differently?

2.Why would casual riders buy Cyclistic annual memberships?

3.How can Cyclists use digital media to influence casual riders to become members?

4.How can your insights drive business decisions?

If we know how casual riders differ from annual members, we can develop a strategy to target casual riders and convert them into annual members.

## DATASET:
The data is on an AWS server where it is easily downloadable and named correctly. I downloaded the previous 11 months data for the year 2022, and stored it locally for the next steps in the analysis processes. The data is current, cited, original but not reliable. There are some null values and outliers in the data.

Note that data-privacy issues prohibits me from using riders’ personally identifiable information. This means that you won’t be able to connect pass purchases to credit card numbers to determine if casual riders live in the Cyclistic service area or if they have purchased multiple single passes.

The files are saved in comma-seperated values (CSV).

Python is used to analyze this data

## DATA COLLECTION
In Data Analytics, the first step is data collection were you gather, obtain, and measure the necessary data from available internal or external data sources, and then compiled the data into an established system. I will be using the Divvy dataset for the case study. The purpose of this script is to consolidate downloaded Divvy data into a single dataframe and then conduct simple analysis to help answer the key question: "In what ways do members and casual riders use Divvy bikes differently?"

Due to the fact that I had multiple datasets that had to be used for the analysis, I had to perform data integration by merging all datasets into a single dataset.

## DATA CLEANING
Created a backup of the merged dataset, to enable me revert to it if I ran into any issue during the cause of my analysis. Changing the data type of 'rideable_type' and 'member_casual' columns to a categorical data type from an object data type. Dropped the 'start_lat', 'start_lng', 'end_lat', 'end_lng' columns from the dataset because they are redundant and its not needed for my analysis. Also the data type for 'started_at' ,'ended_at' were changed to a datetime datatype. I also ran a check to see if thee were any Null values. Apperently there are a lot of null values. Splitted and Extracted the date from the started_at column, converted the start_date datatype to datetime,created a new column to 'day_name' to extract the exact day of the week in words that the rides took place, changed its data type to a categorical data type and created two new columns for the months and year the rides took place.

During the course of my data cleaning, I discovered that 13% of the dataset was made up of null values which is below the 25% maximum, so i dropped them, I also sorted my data by ascending order, checked for duplicate data and finally saved my cleaned data in a new CSV file. With all these tasks performed my dataset was ready for analysis.

## DATA VISUALIZATION
The visualization was done using Tableau, where I imported the cleaned csv data and generated a [dashboard](https://public.tableau.com/views/CyclisticDashboard_16734633881620/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link)



