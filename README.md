# Sentiment-Analysis-on-Amazon-mobile-reviews-dataset-431k-reviews-using-LSTMS

VADER is a sort of sentiment analysis that uses lexicons of sentiment-related terms as its foundation. Each word in the lexicon is graded in terms of whether it is good or negative, and how positive or negative it is: a cheerful mood: 
a composite score of more than 0.5 (compound score > -0.5) and (compound score 0.5) are both considered neutral. -0.5 is the compound score for negative emotion. The total of all lexical ratings that have been harmonised to a range of -1 to 1 is the compound score and

perfomed exploratory data analysis and data preprocessing by finding out the null values and replacing them with unknown because there are 65171 Null values in Brand Name column, if we drop these Null values it means we will drop 65171 row which is a big loss of data. So instead of droping these Null values we will change the Null values into another Unknown brand Name, like this we will save our data

separating the dependent and independent features then finding the stopwords. 

And stemming by changinng the words to its root words, creating a corpus by appending the root words to the corpus list. tokkenizing the words. and building the sequential model using LSTM, adding a embedding layer with dropout vallue 0.33 and adding three dense layers. splitting the data set to train and test sets and traing and testing the data on the model with 10 epochs with batch size of 64. this could take a while having a decent gpu. we can achive 93.5 percentage of the accuracy  with validation loss 0.1735.
