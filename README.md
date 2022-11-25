# Amazon_Vine_Analysis
Big Data analysis using Google Colab, Pyspark, Postgres/pgAdmin, AWS RDS, and SQL

![VineLogo](https://user-images.githubusercontent.com/109354592/204041605-7ec769ed-3454-4fa2-ac8a-338d28b53abb.png)

## Overview

For this project, we'll be analyzing Amazon reviews that have been writted by members from the **Amazon Vine program**, a service the allows both manufactures & publishers to recieve reviews to determine if there are any biaces of their products from **Vine** team members & **Non-Vine** members.

Companies paying a fee to Amazon may provide some free products to it's members, are then required to publish a review to help determine if there are biased feedback between Vine members & Non-members. We'll compare or identify 5 start ratings to overall ratings. This exercise, were asked to choose from 50 datasets and extract, transform & load information into a dataframe to complete or analysis.

## Resources
  * `PySpark`
  * `AWS RDS`
  * `Google Colabortory` - used to import `PySpark`
  * `Postgres` - used to create tables in `SQL` 
  * `amazon_reviews_us_Electronics`
  
## Results
  
  There are over 3 million reviews recorded. To drill down and focus on the reviews that will help us with our analysis we'll filter the dataset by:
   * `Count of Total Votes` greater or equal to 20.
   * `Percent` of `Helpful Votes` to `Total Votes equal` or greater than 50%.
   
![DataGreater20_50](https://user-images.githubusercontent.com/109354592/204043885-6ad6cdf2-730f-45d4-be91-f5046b44e85a.png)
   
Results reduced the total number of reviews from 3M to 50.7K. This allowed us to answer the following questions:

1. How many Vine reviews and non-Vine reviews were there?

Vine members made up only 2.1% (1,080) of the reviews whereas the remaining 97.9% were Non-Vine members (49,659).
