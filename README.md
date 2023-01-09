# ZOMATO-RESTAURANT-CLUSTERING-AND-SENTIMENT-ANALYSIS.
# Problem Statement
Zomato is an Indian restaurant aggregator and food delivery start-up founded by Deepinder Goyal and Pankaj Chaddah in 2008. Zomato provides information, menus and user-reviews of restaurants, and also has food delivery options from partner restaurants in select cities.India is quite famous for its diverse multi cuisine available in a large number of restaurants and hotel resorts, which is reminiscent of unity in diversity. Restaurant business in India is always evolving. More Indians are warming up to the idea of eating restaurant food whether by dining outside or getting food delivered. The growing number of restaurants in every state of India has been a motivation to inspect the data to get some insights, interesting facts and figures about the Indian food industry in each city. So, this project focuses on analysing the Zomato restaurant data for each city in India.

The Project focuses on Customers and Company, you have  to analyze the sentiments of the reviews given by the customer in the data and made some useful conclusion in the form of Visualizations. Also, cluster the zomato restaurants into different segments. The data is vizualized as it becomes easy to analyse data at instant. The Analysis also solve some of the business cases that can directly help the customers finding the Best restaurant in their locality and for the company to grow up and work on the fields they are currently lagging in.

This could help in clustering the restaurants into segments. Also the data has valuable information around cuisine and costing which can be used in cost vs. benefit analysis

Data could be used for sentiment analysis. Also the metadata of reviewers can be used for identifying the critics in the industry.

# Attribute information
## **Zomato Restaurant names and Metadata**
1. Name : Name of Restaurants

2. Links : URL Links of Restaurants

3. Cost : Per person estimated Cost of dining

4. Collection : Tagging of Restaurants w.r.t. Zomato categories

5. Cuisines : Cuisines served by Restaurants

6. Timings : Restaurant Timings

## **Zomato Restaurant reviews**
1. Restaurant : Name of the Restaurant

2. Reviewer : Name of the Reviewer

3. Review : Review Text

4. Rating : Rating Provided by Reviewer

5. MetaData : Reviewer Metadata - No. of Reviews and followers

6. Time: Date and Time of Review

7. Pictures : No. of pictures posted with review

# Project Summary
**This problem contain two dataframes -**

*   **Zomato restaurant  data ** which contains all informations about the restaurants that are available on zomato,Cuisines they serve, per person cost of dining.
*   **User review collection df** which contains the ratings,reviews given by users to different restaurants.

**Clustering **-


*   zomato reaturant data was used  to cluster similar restaurants together based on their ratings ,cuisines they serve  and cost.

*  Mean ratings was taken from user review collection df and then it will be concatenated with zomato restaurant data.

*   K means as well as agglorative clustering both were used for clustering.

*   Silhoutte score was analysed and it was found that 5 and 10 were the optimal number of clusters.

**Sentiment analysis-**


*   There are around 10000 records of reviews and ratings  given by users and from those reviews we need to determine the sentiment of people weather its positive,negative or neutral.
*   Reviews given by customers is a textual information.So to make it perfect for analysis we need to Textual data preprocessing.
The various preprocessing steps that are involved are:

• Tokenization

• Punctuation Mark Removal

• Stop Word Removal

• Lemmatization

*   Word net Lemmatizer was used for lemmatization.

*   Sentiment analysis was done using TextBlob.TextBlob is a python library for Natural Language Processing (NLP).TextBlob actively used Natural Language ToolKit (NLTK) to achieve its tasks. 

*   TextBlob returns polarity and subjectivity of a sentence. Polarity lies between [-1,1], -1 defines a negative sentiment and 1 defines a positive sentiment.

*   TF-IDF vectorizer was used to convert textual informationinto vector form. 

*   people who had positive sentiments had given mean ratings of 4.07 out of 5. People who had negative sentiment have given least mean ratings of only 
1.73 out of 5. People who had neutral sentiments have given mean review in between positive and negative.

*  Logistic regression ,Naive bayes,Random forest,Adaboost,Xgboost,SVM models were used for predicting sentiments using vectorized reviews.

* The best performing models are Xgboost,adaboost and SVM which perform well on both train as well as test data with train accuracy around 0.99 and test accuracy around 0.94.

# Conclusions-

*   Restaurants which have price between 400 -1500 are most in numbers.
*   Collage -Hyatt Hyderabad is the most expensive restaurant and  Amul is the cheapest restaurant along with Mohammedia Shawarma and Sweet Basket.

*   North Indian cuisine is the most famous cuisine among restaurants alongwith chinese, continental and biryani.
*  The Restaurant named 'The Fisherman's Wharf' has been given highest number of tags by zomato and Most frequnt tag given by zomato to restaurants is Great Buffets.

*   AB's absolute barbeque is the highest rated restaurant while Hotel Zara Hi-Fi is the least rated restaurant.
*  So,Delhi -39 and Dine O china had the highest improvement in ratings while The Domino's Pizza  and and own nom nom are restaurants whose ratings 
have gone worse as 1 year has passed.

*   Best silhoutte score is for 5 and 10 number of clusters.
*   people who have positive sentiments have given mean ratings of 4.07 out of 5. People who have negative sentiment have given least mean ratings of only 
1.73 out of 5. People who have neutral sentiments have given mean review in between positive and negative.

*   The best performing models are Xgboost,adaboost and SVM which perform well on both train as well as test data with train accuracy around 0.99 and test accuracy around 0.94.

