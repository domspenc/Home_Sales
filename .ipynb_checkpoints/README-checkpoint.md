# Home Sales

![Risk](image.jpg?raw=true "Risk")

## Overview

In this repository, SparkSQL is used to determine key metrics about home sales data. Spark was also used to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

------------------------------------

#### The following questions were asked:

- What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.

- What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

- What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

- What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

Then, the table was cached. Using the cached data, rerun the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

### Result: 
- Uncached: 1.45 seconds
- Cached: 0.90 seconds

Then, the table was partitioned on the `date_built` field, and a temporary table created for the parquet data. Using this data, rerun the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

### Result: 
- Uncached: 1.45 seconds
- Parqueted 0.87 seconds

Finally, the table was uncached.

----------------------------------



