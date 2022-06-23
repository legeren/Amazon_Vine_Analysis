# Amazon_Vine_Analysis

## Overview of the analysis: 
The purpose of this analysis is to determine if there is any bias toward favorable reviews from Vine members in my chosen product dataset (watches).  In this project, I needed to pick a product review dataset and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I used PySpark for my bias analysis.

- Deliverable 1: [Amazon_Reviews_ETL.ipynb
](https://github.com/legeren/Amazon_Vine_Analysis/blob/22d552a8c4d7778ef19c3f4aa18ad660c4f01c67/Amazon_Reviews_ETL.ipynb)
- Deliverable 2: [Vine_Review_Analysis.ipynb](https://github.com/legeren/Amazon_Vine_Analysis/blob/22d552a8c4d7778ef19c3f4aa18ad660c4f01c67/Vine_Review_Analysis.ipynb)
- Deliverable 3: Results and Summary below

## Results: 
1. How many Vine reviews and non-Vine reviews were there?
   - There were 47 vine reviews and 8,362 non-vine reviews in total for my dataset.
   - ![image](https://user-images.githubusercontent.com/100737452/175182595-77d75545-ee2c-43cf-80cf-f4f142c3b5da.png)


2. How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
   - There were 15 5-star vine reviews and 4,332 5-star non-vine reviews.
   - ![image](https://user-images.githubusercontent.com/100737452/175182663-c732929a-4743-467f-9877-e57c414404b3.png)


3. What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
   - 31.91% of vine reviews were 5-stars while 51.81% of non-vine reviews were 5-stars.
   - ![image](https://user-images.githubusercontent.com/100737452/175182765-8429be93-5245-40ab-9020-4f513350b95d.png)


## Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.
In summary, I do not believe there is enough vine reviews to conclude that there is any positivity bias for reviews in the Vine program based on my chosen dataset.  The vine reviews only represented less than 1% (47 vine reviews/8,409 total reviews) of the total reviews available.  As such, even though 31.91% of vine reviews were 5-stars, it does not skew/influence the overall score of the product.  Besides, more than half of 99% of reviews which were non-vine also reviewed the product at 5-stars.

An additional analysis I could do with the same dataset to support my statement might be to remove the filter for "votes" as this step (see screenshot below) filtered my dataset and may have removed the total number of vine reviews from my analysis which would then let me come to a closer conclusion to determine if there is any positivity bias for reviews.
![image](https://user-images.githubusercontent.com/100737452/175183709-cec4f06d-3f78-404b-a93a-281d5be9b818.png)
