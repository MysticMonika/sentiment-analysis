# sentiment-analysis

The objective of this task is to detect hate speech in tweets. For the sake of simplicity, we say a tweet contains hate speech if it has a racist or sexist sentiment associated with it. So, the task is to classify racist or sexist tweets from other tweets.

It involve following steps:
 ### 1. Tweets Preprocessing and Cleaning:
 
    * The Twitter handles are already masked as @user due to privacy concerns. So, these Twitter handles are hardly giving any       information about the nature of the tweet.
    * We can also think of getting rid of the punctuations, numbers and even special characters since they wouldn’t help in differentiating different kinds of tweets.
    * Most of the smaller words do not add much value. For example, ‘pdx’, ‘his’, ‘all’. So, we will try to remove them as well from our data.
    * Once we have executed the above three steps, we can split every tweet into individual words or tokens which is an essential step in any NLP task.
    * In the 4th tweet, there is a word ‘love’. We might also have terms like loves, loving, lovable, etc. in the rest of the data. These terms are often used in the same context. If we can reduce them to their root word, which is ‘love’, then we can reduce the total number of unique words in our data without losing a significant amount of information.

  ### 2. Story Generation and Visualization from Tweets: 
  
     In this section, we will explore the cleaned tweets text. Exploring and visualizing data, no matter whether its text or any other data, is an essential step in gaining insights.
    * Understanding the common words used in the tweets: A wordcloud is a visualization wherein the most frequent words appear in large size and the less frequent words appear in smaller sizes.
    * After first step we will plot separate wordclouds for both the classes(racist/sexist or not) in our train data.
    * And also understanding the impact of hashtags.

 ### 3. Extracting Features from Cleaned Tweets: 
 
    To analyze a preprocessed data, it needs to be converted into features. Depending upon the usage, text features can be constructed using assorted techniques – Bag-of-Words and TF-IDF.

 ### 4. Model Building: Sentiment Analysis: 
 
      We are now done with all the pre-modeling stages required to get the data in the proper form and shape.
    * building model using bags-of-words feature: ***Accuracy_score is 0.53***
    * building model using Tfidf feature: ***Accuracy_score is 0.544***
    
 ### 5. Last but not the least created API for sentiment analysis of tweets.
 
 
 
