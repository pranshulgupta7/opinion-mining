opinion-mining-sentiment-analysis
==========================
<p>Check simpleDemo.py for a quick demo </p>

Our day-to-day life has always been in influenced by what people think. Ideas and opinions of others have always affected our own opinions. The explosion of Web 2.0 has led to increased activity in Podcasting, Blogging, Tagging, Contributing to RSS, Social Bookmarking, and Social Networking. As a result there has been an eruption of interest in people to mine these vast resources of data for opinions. Sentiment Analysis or Opinion Mining is the computational treatment of opinions, sentiments and subjectivity of text. In this project, various approaches are used to perform a computational treatment of sentiments and opinions. Various supervised or data-driven techniques to Sentiment Analysis like Naive Byes, Support Vector Machine and SentiWordNet approach to Sentiment Analysis.

For example, suppose we are interested in determining whether any product is good or not so good by analysing Twitter messages.

There are primarily two types of appraches for sentiment classification of opinionated texts: 
1. Machine learning based text classifier such as Naive Bayes and Support Vector Machine
2. Natural language processing approach



Machine Learning
=================
Machine learning approach needs a dataset, a classifier to train. Basic idea behind this
approach is that first we collect the data set which can be movie review dataset, twitter
dataset, etc. These data sets are freely available on internet. Then we preprocess the data set
and prepare a training set for our classifier. Using training set we train the classifier, after
training we provide test data set to classifier.



Natural Language Processing
============================

Natural Language Processing approach uses SentiWordNet lexicon, which consists of
positive, negative score for each of the term occuring in WordNet. The implementation is
done by extracting the adjectives out of the sentence and then searching it in the
SentiWordNet to find out its positive, negative score. In this way the total net score of the
sentence is calculated and whichever is greater (either positive or negative) becomes the
review for the sentence.


Twitter API v1.1. is used in get_twitter_data.py  
Add the consumer_key, consumer_secret, access_token, access_oken_secret in config.json file or pass it via command line. 
Try test_twitter_data.py for a sample example.
