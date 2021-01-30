# Amazon_Vine_Analysis
## Overview of the analysis: Explain the purpose of this analysis.

The purpose of this analysis is to perform an ETL analysis on Amazon reviews written by members of the paid Amazon Vine program. The chosen dataset under analysis pertains to Personal Care Appliances. PySpark was used to to determine if there is any bias toward favorable reviews from Vine members in the dataset. The following images shows the dataset divided into tables in pgAdmin PostgreSQL:

(image1)![resources/image1.PNG?raw=true "Title")

(image2)![resources/image2.PNG?raw=true "Title")

(image3)![resources/image3.PNG?raw=true "Title")

(image4)![resources/image4.PNG?raw=true "Title")

## Results: Using bulleted lists and images of DataFrames as support, address the following questions:

- How many Vine reviews and non-Vine reviews were there?
**There were 3 Vine reviews and there were 3094 non-Vine reviews.**

(vinereviews)![resources/paid_vine.PNG?raw=true "Title")

(vineunpaid)![resources/unpaid_vine.PNG?raw=true "Title")

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
**There were 2 Vine reviews that were 5 stars and there were 1704 non-Vine reviews that were 5 stars.**

(vinepaid1)![resources/vine_percent.PNG?raw=true "Title")

(vineunpaid1)![resources/five_star_unpaid.PNG?raw=true "Title")

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
**66.67% of Vine reviews were 5 stars and 55.07% of non-Vine reviews were 5 stars.**

(vinepercent)![resources/vine_percent.PNG?raw=true "Title")

(non_vinepercent)![resources/non_vine_percent.PNG?raw=true "Title")


## Summary
Then, provide one additional analysis that you could do with the dataset to support your statement.

There is a possibility of positivity bias for reviews in the Vine program as the star_rating for items have high ratings ranging from a rating of 3 to a rating of 5. For non-Vine (unpaid) reviews, there was a variation in the star_rating column ranging from a rating of 1 to a rating of 5 as seen in the image of the dataframes below:

(determine_bias)![resources/bias.PNG?raw=true "Title")

There was also the 66.67% of Vine reviews that had 5 star ratings while only 55.07% of non-Vine reviews had 5 star ratings.

**Provide one additional analysis that you could do with the dataset to support your statement.**
One additional analysis is to perform a measure of central tendency analysis (statistics) on the Vine (paid) and non-Vine (unpaid) reviews by using describe() on the paid and unpaid dataframes that were generated in the analysis.

