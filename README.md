# Amazon_Vine_Analysis
## Overview of the Analysis
This project analyzes Amazon reviews written by members of the paid Amazon Vine program.The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project I chose to analyze the video games reviews dataset. I used PySpark to perform the ETL process to extract the dataset, transform the data, connected to an AWS RDS instance, and loaded the transformed data into pgAdmin. Next, I used PySpark to determine if there is any bias toward favorable reviews from Vine members in the video games dataset.


## Results
### Address the following questions to provide support for a reponse to the Summary question:

- How many Vine reviews and non-Vine reviews were there?
I believe the best way to answer this question is to create a line of code to count the total number of reviews that were part of the Vine program (paid) and a second line of code that will count the reviews that were not part of the Vine program (unpaid). The total number of reviews that were part of the Vine program (paid) are 613. The total number of reviews not a part of the Vine program (unpaid): 64968. 

-  How many Vine reviews were 5 stars? 
Total number of 5 star reviews: 15,711 . The number of 5 star Vine member reviews (paid) 222.

- How many non-Vine reviews were 5 stars?
There are 30543 non-Vine (unpaid) 5 star reviews .


-  What percentage of Vine reviews were 5 stars? 
In the photo below 36.215% of the 5 star Vine (paid) reviews were reutrned in the analysis.

- What percentage of non-Vine reviews were 5 stars?
 47.01237532323606% of the 5 star non-Vine (unpaid) reviews were returned in the analysis.



## Summary 
### Is there any positivity bias for reviews in the Vine program? 
This Vine analysis does not take into consideration whether or not those who left a review were able to view previous reviews of others before they made their own review of the video game. Positive reviews may influence others to also leave positive reviews or lessen the negative impact of the review. 

In the case of this analysis, the total percentage of five star reviews (all reviewers) is 48.73%. Over one-third of all video game reviews in the dataset are five star. The large percentage of 5 star reviews, 38.2%, by Vine program members, indicates the possibility of positivity bias. Even though both five star percentages are similar, 47.01237532323606% of non-Vine reviews are five star and 36.215% of reviews by Vine program members, both populations, Vine members and non-Vine members, may be influenced by positivity bias.

One additional analysis I would suggest is more focused on language used by the reviewer to determine the possibility of bias. Is there a similarity in the laguage used by those who provided five star reviews? NLP (Natural Language Processing) would help with classifying text, extracting specific pieces of information contained in the reviews, and summarize the reviews to provide a helpful understanding of the presence or absence of a case for possitivity bias.

this concludes my analysis PEM
