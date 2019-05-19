# Spam-filtering
spam filtering for text messages using python
Maker: Nikhil Betke
modules used: 
1)nltk
2)numpy
3)pandas
4)sklearn
5)sys
dataset used: spam.csv
containing more than 3000 sample messages with labels ham or spam.
modified dataset: newspam.csv
modfied dataset is the prunned dataset with ideal ratio of ham and spam. The prunning is done to get more accurate results.
we used newspam.csv to train our model and it is working fine.

working:
first the data preprocessing is done to prune the dataset to turn it into an ideal dataset. mapping the string values to number to make it suitable to use for machine learning.

We used nltk i.e. natural language toolkit for working with NLP.
We downloaded the common words in English known as stopwords.
Then we used tfidfvectorizer for feature extraction. 
While extracting features we neglected the ordinary stopwords. 
after vectorization we got features of both ham and spam messages.
then we splited the data for training and testing purposes.
then we used SVM, KNN, DecisionTree and NaiveBayes classifiers for predictions. 
All of them gave accuracy over 90%.
In the end there is custom message option where the models can be tested for user defined messages.
