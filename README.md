# AMAZON VINE ANALYSIS

## **Overview of the Analysis**

The Amazon Vine program allows manufacturers and publishers to receive reviews for their products by paying members a fee to publish a review. Vine members are considered paid reviewers while non-Vine members are not paid to publish a review. The company wants to know how the program affect its reviews published.
  
The purpose of the project is to use PySpark to extract Cloud data from Amazon Web Service(AWS), transform the data, connect to AWS RDS instance,load the data into pgAdmin, and provide an analysis on the reviews written on automotive products by both Vine and non-Vine members to determine if there is any biases towards favourable reviews by Vine program members. 

## **Results**

The data was filtered based on total votes equal or greater tha 20 to create a helpful votes and then filtered again using the helpful votes divided by the total votes to be 50% or higher. 

![Analysis Codes](/Images/analysis.png)

- How many Vine reviews and non-Vine reviews were there?
  - Based on the filtered data, the total number of Vine reviews were **82**. The total number of non-Vine member reviews were **24,742**. 

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

  - Based on the filtered data, the Vine reviewers that left a 5-star rating was **33**. Non-Vine members that left a 5-star review was **12,807**

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

  - The Vine reviewers that left a 5-star rating was **33** out of the **82** total reviews representing **40.2%** whereas the non-Vine reviewers with a 5-star rating were **12,807** out of **24,742** representing about **52%**


## **Summary**

In summary, the analysis shows that Vine members, though paid to publish a review did not necessarily submit a 5-star rating. With a lower percentage of 5-star rating among Vine program members than the percentage of 5-star review among non-Vine members, there is not sufficient evidence to support the statement that there is positive bias for reviews in the vine program. There was a higher percentage of non-VINE  members who gave a positive review than members of the Vine program who did. 
Alternatively, negative reviews can be analyzed to support my conclusion. If Vine members has a higher percentage of negative reviews than non-Vine members, it will further show that there is no positivity bias for reviews in the Vine program. 