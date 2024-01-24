# Home_Sales

## Overview

In this challenge we were rquired to carry out a series of data analysis tasks using Apache Spark SQL on a dataset of home sales. The analysis involves reading data from an AWS S3 bucket, creating a SparkSession, and performing various SQL queries to extract insights from the dataset.


## Data Exploration
- A SparkSession was initiated and the home sales dataset was read from an AWS S3 bucket into a DataFrame.
- The DataFrame was then displayed to show the top 20 rows.

- The temporary table ('home_sales') was created for the DataFrame, to enabling the use of Spark SQL queries.


## Data processing
With Spark SQL the following computations were done:

  - The average price for four-bedroom houses sold in each year, rounded to two decimal places 

- The average price for homes with three bedrooms and three bathrooms, grouped by the year they were built, rounded to two decimal places.

- The average price for homes with three bedrooms, three bathrooms, two floors, and a size greater than or equal to 2,000 square feet, grouped by the year they were built.

- The average price of homes for each "view" rating where the homes are greater than or equal to $350,000, and the runtime of the query measured.

- The temporary table 'home_sales' was and checked to comfirm it was cached.

- The query above was repeated using the cached data and the runtime with the uncached version compared.

- The DataFrame was written into parquet and a temporary table for the parquet data was created.

- The same query was ran again using the parquet DataFrame and the runtime was compared with the cached and uncached versions.

- The 'home_sales' temporary table was uncached and checked to confirm if it was no longer cached.
