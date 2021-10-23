# Amazon_Vine_Analysis

## Project Overview
The purpose of this project to analyze Amazon reviews written by members of the paid Amazon Vine program for pet products. performed ETL process, created AWS RDS database with tables in pgAdmin and extracted the dataset into a DataFrame. Next, calculated both Vine and non-Vine reviews to determine if having a paid Vine review makes a difference in the percentage of 5-star reviews.

## Resource

Pet Products Dataset: https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt

## Result

| | Vine review  | Non-Vine review |
| ------------- | ------------- | ------------- |
| Total Number of Reviews | 55  | 10510  |
| The Number of 5-star Reviews | 20 | 6054 |
| Percentage 5-star Reviews | 36% | 58%  |

## Summary
In conclusion, the percentage of 5-star reviews for vine is 36% and for non-vine reviews is 58%, which has markedly different. Based on the statistical result above, I believe that it may not have positivity bias for reviews in the Vine program. However, in compare, the total number of vine review (55 records) is way less than non-vine review (10510 records), it would be better if we can collect more vine reviews for this analysis. On the other hand, I would suggest that we can filter the data by adding "verified_purchase", the review is on a verified purchase. It's meaning that the reviews were probably written after they use the product, so the result of this analysis would be more precise.
