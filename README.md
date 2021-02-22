# Amazon_Vine_Analysis
- PySpark Cloud ETL Application

## Purpose 
- Extract online database that contains Amazon review dataframe
- Load cleaned and filtered dataframes into PostgresSQL (pgAdmin)
- Evaulate if there is any bias in the 5-star review data for paid and unpaid reviewers

##  Resources
- pgAdmin
- PySpark
- AWS, RDS
- Amazone Vine Review dataset: Home Improvement 

##  Data Review

### How many Vine reviews and non-Vine reviews were there?
- Vine reviews: 266
- Non-Vine reviews: 38,829

### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
- Vine Reviews (5 Stars): 125
- Non-Vine Reviews (5 Stars): 18,246

### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
- Proportion of Vine reviews that were 5 stars: 46.99248120300752%
- Proportion of non-Vine reviews that were 5 stars: 46.99065131731438%

##  Summary
Based on the data a few observations can be made. First, about 47% of reviews were 5-star indicating that there is a positivity bias - meaning that people tend to give high ratings. Nearly half being at 5 stars means that ratings are not equally distributed across each rating (1 though 5 star). The second observation is that Vine (paid) and non-Vine (unpaid) reviews have about the same proportion of 5-star ratings, meaning that the paid reviewers are likely to be representative of the overall review data population. An additional analysis that would help to statistically support these statements is a student t test to see if the 5-star data proportions for paid and un-paid reviews are not statistically different. 