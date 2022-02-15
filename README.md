# Analytics-vidya-jobathon-feb
In the jobathon, our task was to calculate the video engagement score for each user

**introduction**

The objective of the hackathon was to develop a machine learning approach to predict the engagement between a user and a video. The training data already had an engagement score feature, which was a floating-point number between 0 and 5. This considerably simplified matters, as in recommender systems, calculating the engagement score is often more challenging than predicting them. The challenge, therefore, was to predict this score based on certain user related and video related features

There was no missing values present in the dataset and the dataset was almost balanced.

**feature engineering**

there are two features present in the dataset that has catagorical features we need to encode those features such that they will give numeric values. we have used one cot encoding for that.
whne we are plotting the corelation matrix we have seen that some of the features are highly corelated and thier contribution to the engagement score was too low, So we can remove the those columns. After feature engineering i have used **randomForestRegressor** algorithm for predicting the engagement score.

**r2 score**

the final r2 score on test data was 0.42.

**test result**
I have store the test dataset engagement score to the saparate CSV file. This file contains the raw_id and the respective engagement score.

**future scope**
