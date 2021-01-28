# Twitter-Sentiment-Analysis
Sentiment Analysis by training a Naive Bayes classifier to predict sentiment from thousands of Twitter tweets.
Dataset Source: https://www.kaggle.com/bhuwanesh340/predicting-tweet-sentiments

Only the train.csv file was used in this project.


## The Dataset

The dataset had positive tweets flagged by 0 and negative tweets flagged by 1 in the label column as shown below: (Since the ID column was of no use, it was removed from the dataset)

![alt text](https://github.com/alizaazizlakho/Twitter-Sentiment-Analysis/blob/main/pictures/dataset.png)

Next, to get an idea of the total number of positive and negative tweets, I used Seaborn to plot a count plot:

![alt text](https://github.com/alizaazizlakho/Twitter-Sentiment-Analysis/blob/main/pictures/distribution%20plot.png)

Next, all the tweets were converted from a dataframe to a list so that wordclouds could be plotted. Below you will find three wordclouds:

1) Most commonly words used in the tweets in this dataset

![alt text](https://github.com/alizaazizlakho/Twitter-Sentiment-Analysis/blob/main/pictures/Wordcloud.png)

2) Most commonly words used in the positive tweets in this dataset

![alt text](https://github.com/alizaazizlakho/Twitter-Sentiment-Analysis/blob/main/pictures/Wordcloud1.png)

2) Most commonly words used in the negative tweets in this dataset

![alt text](https://github.com/alizaazizlakho/Twitter-Sentiment-Analysis/blob/main/pictures/Wordcloud2.png)

After cleaning the tweet (by removing punctuation and stopwords) I performed count verctorization and then I trained my model on Naive Bayes Classifier where I only used 10% of the data (due to limitations on the Memory that I could use).

Following is the heatmap of the Confusion Matrix:

![alt text](https://github.com/alizaazizlakho/Twitter-Sentiment-Analysis/blob/main/pictures/Confusion%20Matrix.png)

And the classfication report inidcating precision and accuracy of the model when it was tested on the remaining values in train.csv

![alt text](https://github.com/alizaazizlakho/Twitter-Sentiment-Analysis/blob/main/pictures/Classification%20Report.png)
