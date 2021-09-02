# Big-data-challenge

## Amazon reviews

###  Many of Amazon's shoppers depend on product reviews to make a purchase. Amazon makes these datasets publicly available. However, they are quite large and can exceed the capacity of local machines to handle. However, they are quite large and can exceed the capacity of local machines to handle. One dataset alone contains over 1.5 million rows; with over 40 datasets, this can be quite taxing on the average local computer

First of All we have to Extract, Transform and Load the data:

Extraction from: [Amazon_Reviews](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)

Let's count rows:

Videogames reviews | 1785997
------------------ | -------

Now, we have to tranform it into a SQL schema with this frame:

* Product table
* Customers table
* Vine table

[SQL_SCHEMA](https://github.com/greaterpablo/big-data-challenge/blob/main/Resources/schema.sql)

Now push to AWS RDS instance

Look at the [Solution](https://github.com/greaterpablo/big-data-challenge/blob/main/Level-1/level_one_solution.ipynb)

In Amazon's Vine program, reviewers receive free products in exchange for reviews.

But are Vine reviews truly trustworthy? Your task is to investigate whether Vine reviews are free of bias. Use either PySpark or—for an extra challenge—SQL to analyze the data.

We need to Filter Votes

Now to describe Stats 

Som statics: 
* Percentage of 5-Stars reviews among Vine Reviews

Vine Reviewrs | #
------------- | -
Number of paid reviews | 94
Number of paid five star reviews | 48
Percantage of paid reviews that are five stars | 51.06%

* Percentage of 5-Stars among Vine-Reviewers

