# Rockbuster-SQL-Analysis
## SQL is used to answer business and inventory questions for Rockbuster Video rental company in order to compete with bigger platforms like Netflix and Amazon. The video company plans to launch an online service and needs to look at consumer data to strategize how to do so effectively. 

## Join Statement


## CTE
### First, I created a CTE table (top_countries) with the ‘WITH’ function and defined our first condition, the lowest level of filtered data: The “Country” condition. Just as before, this filters our data by the COUNT of customer IDs in DESC order. Next, I created a CTE (top_cities ) for the “City” condition whichDESC as well, but only pertains to the countries we’ve previously selected. Thus, our data passes through another filter. Finally, we have the “top_customers” CTE, which selects the customer IDs and aggregate SUM function, joins everything together, sorts by cities, and then displays in DESC order of total amount paid. Lastly, we have our main statement. Here we connect our first two tables together with join functions and connect our subquery by setting the customer_id’s equal. Our three columns are displayed by country, amount of distinct customers per country and amount of top 5 customers per country.
