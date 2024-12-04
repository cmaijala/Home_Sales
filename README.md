# Home_Sales

## Home Sales Analysis
### Overview
In this project, I used SparkSQL to analyze home sales data, extracting key metrics such as average prices based on various attributes like the number of bedrooms, bathrooms, square footage, and the year the home was built. Additionally, I explored how partitioning, caching, and uncaching data can affect query performance.

## Tasks Completed
1.) Data Processing:

  * Loaded the home_sales_revised.csv file into a Spark DataFrame.
  * Created a temporary table named home_sales.
    
2.) Queries:

  * Calculated the average price for a four-bedroom house sold per year.
  * Calculated the average price for homes built in each year with three bedrooms and three bathrooms.
  * Calculated the average price for homes with three bedrooms, three bathrooms, two floors, and at least 2,000 square feet, built in each year.
  * Determined the average price of homes per "view" rating, for homes with an average price greater than or equal to $350,000, and measured query runtime.
    
3.) Performance Optimization:

  * Cached the home_sales temporary table to improve query performance.
  * Compared query runtime between cached and uncached data.
  * Partitioned the data by the date_built field and created a temporary table for the parquet data.
  * Uncached the table and verified that it was successfully uncached.
    
## Technologies Used
  * PySpark: For data manipulation and analysis using SparkSQL.
  * Parquet: For efficient data storage and partitioning.
    
## Performance Insights
  * Caching significantly improved query performance for complex queries.
  * Partitioning by date_built allowed for better organization and faster querying on the dataset.
    
## Repository
The completed notebook is stored in this repository, showcasing both the code and analysis of the data.
