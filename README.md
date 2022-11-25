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

**1. How many Vine reviews and non-Vine reviews were there?**
   * Vine members made up only 2.1% (1,080) of the reviews whereas the remaining 97.9% were Non-Vine members (49,659).
   
![VineNonVineTotal](https://user-images.githubusercontent.com/109354592/204044158-957f49b6-de0a-4006-8f98-04e8e1d586ac.png)

![Vine](https://user-images.githubusercontent.com/109354592/204044256-0e9bac6a-c97a-47eb-8a06-59726d5ac7d7.png)

![NonVine](https://user-images.githubusercontent.com/109354592/204044270-9faac817-d643-42c7-be46-b4195bd3e707.png)

**2.How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?**
   * **Vine** members gave _454_ out of _1,080_ reviews a `5 star rating`.
   * **Non-Vine** members gave _23,034_ out of _49,659_ reviews a `5 star rating`.
   
**3.What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?**  
   * _`42%`_ of the reviews for **Vine** members were rated `5 stars`.
   * _`46.4%`_ of the reviews for **Non-Vine** members were rated `5 stars`.
  
## Summary


 







