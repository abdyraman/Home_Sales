I used SparkSQL to determine key metrics about home sales data. 
Then I used Spark to create temporary views, partition the data, cache and uncache a temporary table, and verified that the table has been uncached.
Steps Accomplished:

1. A Spark DataFrame was created from the dataset.
2. A temporary table of the original DataFrame was created.
3. A query was written to return the average price, rounded to two decimal places, for a four-bedroom house that was sold in each year.
4. Another query was written to return the average price, rounded to two decimal places, of a home with three bedrooms and three bathrooms.
5. A query was formulated to return the average price of a home with three bedrooms, three bathrooms, two floors, and a size greater than or equal to 2,000 square feet for each year built, rounded to two decimal places.
6. A query was composed to return the view rating for the average price of homes that are greater than or equal to $350,000, rounded to two decimal places. The output also displayed the run time for this query.
7. A cache of the temporary "home_sales" table was created and verified.
8. The query from step 6 was executed on the cached temporary table, and the run time was computed.
9. A partition of the home sales dataset by the "date_built" field was created, and the formatted parquet data was read.
10. A temporary table of the parquet data was created.
11. The query from step 6 was run on the parquet temporary table, and the run time was computed.
12. The "home_sales" temporary table was uncached and confirmed.
