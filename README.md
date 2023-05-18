In this challenge, we used  SparkSQL to determine key metrics about home sales data. 
We used Spark to create temporary views, partition the data, cache and uncache a temporary
table, and verify that the table has been uncached. We used Colab.

* Imported the necessary PySpark SQL functions for this assignment.

* Read the ```home_sales_revised.csv``` data into a Spark DataFrame.

* Created a temporary table called ```home_sales```.

Answered the following questions using SparkSQL:

1. What is the average price for a four-bedroom house sold for each year? Rounded off answer 
to two decimal places.

2. What is the average price of a home for each year it was built that has three bedrooms and 
three bathrooms? Rounded off answer to two decimal places.

3. What is the average price of a home for each year that has three bedrooms, three bathrooms, two
floors, and is greater than or equal to 2,000 square feet? Rounded off answer to two decimal
places.

4. What is the "view" rating for homes costing more than or equal to $350,000? Determined the run 
time for this query, and rounded off answer to two decimal places.

* Cached temporary table ```home_sales```. Checked if temporary table was cached.

* Using the cached data, ran the query that filters out the view ratings with an average price of
greater than or equal to $350,000. Determined the runtime and compared it to uncached runtime.

* Partitioned by the "date_built" field on the formatted parquet home sales data.

* Created a temporary table for the parquet data.

* Ran the query that filters out the view ratings with an average price of greater than or equal 
to $350,000. Determined the runtime and comparde it to uncached runtime.

* Uncached the ```home_sales``` temporary table.

* Verified that the ```home_sales``` temporary table is uncached using PySpark.

* Downloaded ```Home_Sales.ipynb file``` Colab file