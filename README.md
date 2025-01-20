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

This project applies on the 5 dimensions of Big Data ( **The 5 Vs**):
1. Volume (The scale of data being processed)
2. Velocity (The speed at which data is generated and processed)
3. Variety (The diversity of data types)
4. Veracity (The reliability and quality of data through data cleaning and preprocessing steps)
5. Value (The actionable insights derived from the data)

**Analysis Results:**

**Dataset Information**
The dataset used for this analysis was sourced from Kaggle and contains approximately 10,000 rows of Tesla-related tweets.

**Sentiment Analysis of Tesla Tweets**
The majority of people expressed neutral thoughts about Tesla based on sentiment analysis conducted on tweets. This conclusion is drawn from the analysis of tweet content and the number of likes each tweet received.

**Clustering Insights**
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
**Key Insights**
Most tweets express neutral sentiment about Tesla.
Engagement (likes) is highest for positive tweets, followed by neutral and negative ones.
Clustering confirmed a strong alignment between sentiment labels and engagement trends.

**Project Overview**

This project focuses on analyzing Tesla-related tweets to understand public sentiment and the relationship between sentiments and engagement (likes). The analysis involves data collection, cleaning, sentiment analysis, clustering, and visualizations. Below is a breakdown of the workflow:

**1. Data Acquisition**
Source: The dataset was sourced from Kaggle, containing approximately 10,000 rows of Tesla-related tweets.
Storage: Data was fetched from MongoDB Atlas using Python's pymongo library.
**2. Data Cleaning**
Removed unnecessary columns, duplicates, and rows with missing values.
Cleaned the tweet text by:
Removing URLs, mentions, hashtags, and special characters.
Converting text to lowercase for uniformity.
**3. Sentiment Analysis**
Conducted using the TextBlob library to classify tweets into Positive, Neutral, or Negative sentiments.
Updated the MongoDB collection with sentiment labels.
**4. Clustering and Correlation Analysis**
**Clustering:**
Created TF-IDF vectors from cleaned tweets to quantify the textual data.
Applied K-Means clustering to group tweets into three clusters corresponding to Positive, Neutral, and Negative sentiments.
**Correlation Analysis:**
Calculated the average number of likes for each sentiment group to identify engagement trends.
**5. Visualizations**
