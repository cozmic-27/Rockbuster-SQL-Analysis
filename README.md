# Rockbuster-SQL-Analysis
#### SQL is used to answer business and inventory questions for Rockbuster Video rental company in order to compete with bigger platforms like Netflix and Amazon. The video company plans to launch an online service and needs to look at consumer data to strategize how to do so effectively. Using SQL, data is analyed to answer key questions in regards to revenue, customer geographical location, rental durations, popular genres and so on. Using these insights, Rockbuster Stealth can craft more accurate customer profiles to drive revenue.

# Key Questions

#### 1. Which movies contributed the most/least to revenue gain?
#### 2. What was the average rental duration for all videos?
#### 3. Which countries are Rockbuster customers based in?
#### 4. Where are customers with a high lifetime value based?
#### 5. Do sales figures vary between geographic regions?

# SQL Breakdown

## Join Statement
#### Querry sorts cities in each country by descending order based on number of customers. Data is grouped by each city and country and their respective amount of customers.

## CTE
#### First, I created a CTE table (top_countries) with the ‘WITH’ function and defined our first condition, the lowest level of filtered data: The “Country” condition. Just as before, this filters our data by the COUNT of customer IDs in DESC order. Next, I created a CTE (top_cities ) for the “City” condition whichDESC as well, but only pertains to the countries we’ve previously selected. Thus, our data passes through another filter. Finally, we have the “top_customers” CTE, which selects the customer IDs and aggregate SUM function, joins everything together, sorts by cities, and then displays in DESC order of total amount paid. Lastly, we have our main statement. Here we connect our first two tables together with join functions and connect our subquery by setting the customer_id’s equal. Our three columns are displayed by country, amount of distinct customers per country and amount of top 5 customers per country.

# Data Tools

#### Rockbuster relational database management system and Postgre SQL were used for analysis. Tableau was used for visualizations.
[Tableau Visualizations](https://public.tableau.com/app/profile/zach.ungerman/viz/RockbusterDataVisualizations_17238265988350/Story1)
