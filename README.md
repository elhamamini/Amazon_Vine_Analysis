# Amazon_Vine_Analysis
### Positivity Bias in Vine Member Reviews
Analyst: <code><i> Elham Amini, Columbia University Data Analytics Bootcamp</i></code><br />
Systems Used: <i><code> PySpark with Google Colaboratory, PostgreSQL accessing AWS RDS instance, Python 3.9 with Pandas and Numpy in Jupyter Notebook </i></code><br />
Data Source: <i><code>Amazon Analyitics</code></i>

## Overview
#### Abstract
The team has been tasked to analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

The intent of this analysis is to determine if there is bias toward favorable reviews from Vine members in this dataset.
<br />
## Results
#### Method for Selecting Data
This analysis is for products categorized as Health & Personal Care. Sample size (5.3MM records) afforded the analysis of the top reviews according to number of votes on what is rated as excellent products. Dataset is condensed to only records that are more than 20 votes on the product review, and a minimum of 5 stars awarded by the reviewer.<br />

From the findings of the study of this subset, we find:
  - The study produced a sample group of 480 Vine member reviews, and 124,824 non-member reviews.
  - The study found that there were 214 five-star reviews by Vine members, and 71,737 by non-members
  - Vine subscribers award 5 stars to a product with lower frequency than non-subscribers
    - Vine members appear to be more stringent with their reviews as they award 5 stars at a rate of 44.58%
    - Non-subscribers appear to be less stringent and award 5 stars at a higher rate of 57.47%<br />

<img width="500" alt="results" src="https://user-images.githubusercontent.com/84740997/135160761-b60b6ee5-5e46-4275-b83e-4b4953d10ae1.png"><img width="600" alt="stackedbar" src="https://user-images.githubusercontent.com/84740997/135168804-f0cfb09b-86ce-412b-aa1b-01a75314728e.png">
<br />
## Summary
#### Bias in Vine Reviews
In summary, we have not found a positivity bias in Vine reviews. Regarding overall 5-star review tendencies, in fact it appears Vine members are less inclined to promote a product with 5-stars. Vine members take their positions with more care, and sincerity.<br />

To further expand this study to take a deeper dive, expand the subset to 4 as well as 5 star reviews. The larger dataset would afford a different perspective.
