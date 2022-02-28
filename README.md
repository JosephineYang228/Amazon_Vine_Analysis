# Amazon_Vine_Analysis
## Overview of the analysis
This project is designed to analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. In this project, I picked one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin, in order to determine if there is any bias toward favorable reviews from Vine members in your dataset.

## Results
 - How many Vine reviews and non-Vine reviews were there?  
 There were 94 Vine reviews and 40471 non-Vine reviews.  
 ![total_paidR](https://github.com/JosephineYang228/Amazon_Vine_Analysis/blob/80c5303387cf42faa27c637736a3f620579e88ea/image/total_paidR.png)  
 ![total_unpaidR](https://github.com/JosephineYang228/Amazon_Vine_Analysis/blob/80c5303387cf42faa27c637736a3f620579e88ea/image/total_unpaidR.png)
 
 - How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?  
 There were 48 Vine reviews and 15663 non-Vine revews were 5-Star.  
 ![5-SR](https://github.com/JosephineYang228/Amazon_Vine_Analysis/blob/80c5303387cf42faa27c637736a3f620579e88ea/image/5-SR.png)  
 ![U5-SR](https://github.com/JosephineYang228/Amazon_Vine_Analysis/blob/80c5303387cf42faa27c637736a3f620579e88ea/image/U5-SR.png)  
 
 - What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?  
 The percentage of 5-Star Vine reviews was 51.06% and the percentage of 5-Star non-Vine reviews was 38.70%.  
 ![5-SP](https://github.com/JosephineYang228/Amazon_Vine_Analysis/blob/80c5303387cf42faa27c637736a3f620579e88ea/image/5-SP.png)  
 ![U5-SP](https://github.com/JosephineYang228/Amazon_Vine_Analysis/blob/80c5303387cf42faa27c637736a3f620579e88ea/image/U5-SP.png)
 
## Summary
I do believe there exist positivity bias for reviews in the Vine program according to the 5-Star review percentage comparison. There were 51.06% of the Vine reviews were 5 Star while only 38.70% of the non-Vine reviews were 5-Star.  
### Additional analysis to support
I suggest to add an analysis for the mode and mean value of Vine and non-Vine customrers. Thus we could know what's the ratings of video games products from the Vine and non-Vine customers' view and push notifications in a more targeted way.
