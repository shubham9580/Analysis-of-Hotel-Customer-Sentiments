# Analysis-of-Hotel-Customer-Sentiments
Sentiment analysis is part of the Natural Language Processing (NLP) techniques that consists in extracting emotions related to some raw texts. This is usually used on social media posts and customer reviews in order to automatically understand if some users are positive or negative and why. The goal of this study is to show how sentiment analysis can be performed using python. Here are some of the main libraries we will use:

NLTK: the most famous python module for NLP techniques.
Gensim: a topic-modeling and vector space modeling toolkit.
Scikit-learn: the most used python machine-learning library.
We will use here some hotel review data. Each observation consists of one customer review for one hotel. Each customer review is composed of textual feedback of the customer's experience at the hotel and an overall rating.

For each textual review, we want to predict if it corresponds to a good review (the customer is happy) or to a bad one (the customer is not satisfied). The review's overall ratings can range from 2.5/10 to 10/10.

In order to simplify the problem we will split those into two categories:

bad reviews have overall ratings < 5
good reviews have overall ratings > = 5

About Dataset
Acknowledgements
The data was scraped from Booking.com. All data in the file is publicly available to everyone already. Please be noted that data is originally owned by Booking.com.
Data Context
This dataset contains 515,000 customer reviews and scoring of 1493 luxury hotels across Europe. Meanwhile, the geographical location of hotels are also provided for further analysis.
Data Content
The csv file contains 17 fields. The description of each field is as below:

Hotel_Address: Address of hotel.
Review_Date: Date when reviewer posted the corresponding review.
Average_Score: Average Score of the hotel, calculated based on the latest comment in the last year.
Hotel_Name: Name of Hotel
Reviewer_Nationality: Nationality of Reviewer
Negative_Review: Negative Review the reviewer gave to the hotel. If the reviewer does not give the negative review, then it should be: 'No Negative'
Review_Total_Negative_Word_Counts: Total number of words in the negative review.
Positive_Review: Positive Review the reviewer gave to the hotel. If the reviewer does not give the negative review, then it should be: 'No Positive'
Review_Total_Positive_Word_Counts: Total number of words in the positive review.
Reviewer_Score: Score the reviewer has given to the hotel, based on his/her experience
Total_Number_of_Reviews_Reviewer_Has_Given: Number of Reviews the reviewers has given in the past.
Total_Number_of_Reviews: Total number of valid reviews the hotel has.
Tags: Tags reviewer gave the hotel.
days_since_review: Duration between the review date and scrape date.
Additional_Number_of_Scoring: There are also some guests who just made a scoring on the service rather than a review. This number indicates how many valid scores without review in there.
lat: Latitude of the hotel
lng: longtitude of the hote
