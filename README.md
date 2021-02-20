# **AMAZON VINE REVIEWS**
## **PROJECT OVERVIEW**

This project is about the analysis of *Amazon Vine* program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. 
The idea of this analysis is to determine if there is any bias toward favorable reviews from Vine members? I have used PySpark to extract, transform and load the dataset from Amazon's reviews on "Shoes", using Google Colab.

## **RESULTS**

### **Number of Vine and Non-Vine Reviews**

<img src='number of reviews.PNG'><img>

As evident from above snippet, there are 22 reviews by Vine members and 26987 reviews by the non-vine members.

### **Number of 5 Star reviews in Vine and Non-Vine categories**

<img src='number of 5 star reviews.PNG'><img>

There are 13 '5-star' reviews by Vine members and 14475 '5-star' reviews by non-vine members.

### **Percentage of 5 Star reviews in each category**

<img src='percentage of 5 star reviews.PNG'><img>

As shown in the above code snippet, 59% reviews by Vine members were 5 star and 53.6% reviews were 5 star by non vine members.

## **SUMMARY**

The difference between 5 star reviews by Vine and Non-Vine members is not that big (59% vs 53.6%-only about 5 base points difference) so by looking at this data, we can deduce that there is no positive bias or the motivation for the members to give 5 star reviews if they are paid for this. 

However our data has very less number of reviews by Vine members (only 22) and number of 5 star reviews (13) so making a general conclusion would not be that effective. It would be prudent to have higher number of reviews to make a solid conclusion. 

### **Additional Analysis**

To dig deeper into our conclusion that there is no positive bias in the given data based on "5 Star" reviews only, I have expanded my range to 4 star reviews as well. The following code snippet shows the result if we have 4 and 5 star reviews combined:

<img src='additional analysis.PNG'><img>

It is evident that if we combine 4 and 5 star reviews then the percentage of positive reviews by Vine members is 86% while that of Non-Vine members is 68.6%. Now there is relatively bigger difference of positive reviews by Vine members as comapred to Non-Vine. So we can say that percentage of positive reviews if they are paid is much higher than if the reviews are unpaid.
