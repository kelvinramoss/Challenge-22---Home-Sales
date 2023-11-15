# Challenge-22---Home-Sales

For this task, you'll leverage your SparkSQL expertise to extract crucial metrics from home sales data. You'll employ Spark to generate temporary views, segment the data, store it in memory temporarily, remove it from memory, and confirm the removal of the stored table.

## Instructions

1. Rename the Home_Sales_starter_code.ipynb file as Home_Sales.ipynb.

2. Import the necessary PySpark SQL functions for this assignment.

3. Read the home_sales_revised.csv data in the starter code into a Spark DataFrame.

4. Create a temporary table called home_sales.

5. Answer the following questions using SparkSQL:

    - What is the average price for a four-bedroom house sold for each year? Rounding to two decimal places. 

    - What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Rounding to two decimal places.

    - What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Rounding to two decimal places.

    - What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and rounding to two decimal places.

6. Cache your temporary table home_sales.

7. Check if your temporary table is cached.

Using the cached data:

1. Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

2. Partition by the "date_built" field on the formatted parquet home sales data.

3. Create a temporary table for the parquet data.

Using the parquet data:

1. Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

2. Uncache the home_sales temporary table.

3. Verify that the home_sales temporary table is uncached using PySpark.

4. Download your Home_Sales.ipynb file and upload it into your "Home_Sales" GitHub repository.

