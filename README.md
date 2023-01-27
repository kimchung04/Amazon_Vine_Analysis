# Amazon Vine Analysis
## Overview of the Analysis
In this project, we analyse wether Amazon reviews written by members of the paid Amazon Vine program are biased. For this, we chose to analyse the Automotive reviews dataset provided by Amazon at [Automotive Reviews](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Automotive_v1_00.tsv.gz) using PySpark for improved performance. In order to get a better analysis, we filtered the reviews to those who have over 20 votes and whose helpful votes are at least 50% of the total votes.

## Results
We obtainedthe following results:
1. Total Votes:

    |Vine Votes| Non Vine Votes|
    |:--------:|:-------------:|
    |76        | 23015         |

2. 5 Stars Reviews:
    |Vine Votes| Non Vine Votes|
    |:--------:|:-------------:|
    |30        | 11914         |

3. Percentage of 5 stars:
    |Vine Votes| Non Vine Votes|
    |:--------:|:-------------:|
    |39.47%    | 51.77%        |

## Summary
Bias could be in favor or against the product. What we can observe from the non-members reviews are giving the products 5 stars in just over 50% of the cases while the members in only 40%. This could be explained by the fact that members are more rigorouse when evaluating a product, so it should come as no surprise that the extremes, 1 and 5 stars, should have a lower percentage of appearance in the Vine member reviews than in the non-members.
The following histogram of the stars assigned by members and non-members supports the idea of giving out extreme stars more easily by the non-members.
![](images/feq.png)
Finally, from this dataset, there is no conclusive evidence to suggest that there is bias by the Vine members.
