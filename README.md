# Big-Data-Management-and-Processing
Big Data Management and Processing Homework 

#You may find below the url for Sentiment Analysis from tweets about Tesla. 
http://localhost:8888/notebooks/Big%20Data%20Management%20and%20Processing%20Homework%202%20_%20Exc4.ipynb

- Download MongoDB Compass
    - Install MongoDB Compass from the official website.
- Connection between MongoDB Compass & MongoDB Atlas
  In MongoDB Atlas follow the following steps:
    - Create a MongoDB Atlas Cluster.
    - Set Up Database User.
    - Whitelist Your IP Address (Here Google Colab ip).
    - Get the Connection String.
    - Connect Using MongoDB Compass
**Important Note:**
Each time the connection is interrupted (e.g., when Google Colab resets), the IP address will change.
You will need to update the whitelisted IP address in MongoDB Atlas before rerunning the notebook or reconnecting.


**Analysis Results:**
Sentiment Analysis of Tesla Tweets
The majority of people expressed neutral thoughts about Tesla based on sentiment analysis conducted on tweets. This conclusion is drawn from the analysis of tweet content and the number of likes each tweet received.

Clustering Insights
Through clustering, I observed the following relationship between likes and sentiment:

Positive tweets receive the highest number of likes.
Neutral tweets receive an average number of likes.
Negative tweets receive the fewest likes.
Correlation Between Likes and Sentiment
The following table summarizes the correlation between sentiment categories and the number of likes:

Predicted Sentiment	Average Likes
Negative ->	0.891652
Neutral	-> 1.039401
Positive -> 3.522094
These results highlight the strong engagement with positive sentiment tweets about Tesla compared to neutral or negative ones.
