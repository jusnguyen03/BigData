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
Please check link https://colab.research.google.com/drive/1ap3upRLC4GbbhUF6YCFUT4KlFaxi1Rqf for the code

The results of the data in comparison, after splitting the all the reviews to vine (paid) and non-vine (unpaid) are as follows:
- total reviews (paid) 103 vs (non-paid) 4,098,755
- total helpful votes (paid) 103 vs (non-paid) 4,098,755
- number of 5-star reviews that are helpful votes (paid) 74 vs (non-paid) 2,693,601

In conclusion, I can say that the vine (paid) reviews are trustworthy. Although, in sheer volume of the total reviews and helpful votes, non-vine (unpaid) has a lot more of a sample size compared to vine (paid). The reason I can conclude that the vine reviews are trustworthy is because of the quality of the reviews. The percentage of the average of helpful votes relative to that of the total votes for paid is much higher than the unpaid.  As shown in the snapshot below in comparison, the paid helpful votes number are much closer to the total votes number than the unpaid. 

![](https://github.com/jusnguyen03/BigData/blob/master/average.png)
