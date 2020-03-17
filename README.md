# BigData

## Project Overview
I will be diving into what constitutes big data and how it's handled. I will be:
  - Define big data and describe the challenges associate with it.
  - Define Hadoop and name the main elements of its ecosystem.
  - Explain how MapReduce processes data.
  - Define Spark and explain how it processes data.
  - Describe how NLP collects and analyzes text data.
  - Explain how to use AWS Simple Storage Service (S3) and relational databases for basic cloud storage.
  - Complete an analysis of an Amazon customer review.

## Resources
- Data Source: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz , user_data.csv, user_payment.csv
- Software: Amazon Web Services (AWS), Colab Notebooks, pgAdmin 4, RDS

## Challenge Overview
In this challenge, I will perform the ETL process completely in the cloud and upload a DataFrame to an RDS instance. Then I will use PySpark to perform a statistical analysis of the selected data.

The goals for this challenge are:
  1. Perform ETL on one of the review datasets.
  2. Store your results on an AWS RDS database.
  3. Determine if reviews are biased using PySpark or SQL with the appropriate statistical methods.


## Challenge Submission
Please check link https://colab.research.google.com/drive/1N-vSnf-tO9d0jsQF6a4ojT9R_ugpKkOl for the code

The results of the data in comparison, after splitting the all the reviews to vine (paid) and non-vine (unpaid) are as follows:
- total reviews (paid) 4 vs (non-paid) 3,944,284
- number of 5-star reviews that are helpful votes (paid) 2 vs (non-paid) 2,395,123

In conclusion, due to the amount in volume of the total reviews and helpful votes, non-vine (unpaid) has a lot more of a sample size compared to vine (paid), I deem the vine reviews to not trustworthy. Although, the quality of the vine reviews seem to be great, they are still not trustworthy, because of the very small of amounts that exist (only 4). Below is also a snapshot of the average helpful votes compared to the average total votes for each rating score (1-5) for both vine and non-vine.

![]()
