# Amazon_Vine_Analysis

## Overview

ETL process using PySpark into AWS RDS. A dataset of Amazon reviews for video games is transformed and loaded into a database. A quick analysis is then conducted, investigating the Vine program which provides products to users who then publish reviews.

## Results

### Dataframes

The following are the dataframes containing the Vine and non-Vine reviews:

![1](/Results/vine_df.png)

![2](/Results/non_vine_df.png)

### Analysis

The following are the analysis calculations for the Vine and non-Vine reviews:

![3](/Results/vine_calc.png)

![4](/Results/non_vine_calc.png)

* There are 94 Vine program reviews; there are 40471 unpaid reviews.
* There are 48 Vine program five star reviews; there are 15663 unpaid five star reviews.
* Five star reviews make up 51.1% of the Vine reviews; five star reviews make up 38.7% of the unpaid reviews.

## Summary

* There appears to be a bias towards higher reviews in the Vine program. This is supported by 51.1% of the Vine reviews being five star reviews, while only 38.7% of the unpaid reviews being five star reviews.
* As an additional test to support the positivity bias for reviews in the Vine program, a two-sample t-test could be conducted to determine whether there is a statistical difference between the means of the Vine and non-Vine review samples.