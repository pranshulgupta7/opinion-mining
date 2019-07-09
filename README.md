opinion-mining-sentiment-analysis
==========================
<p>Check simpleDemo.py for a quick demo </p>

There are primarily two types of appraches for sentiment classification of opinionated texts: 
1. Machine learning based text classifier such as Naive Bayes and Support Vector Machine
2. Natural language processing approach



Machine Learning Approach
==========================
Machine learning approach needs a dataset, a classifier to train. Basic idea behind this
approach is that first we collect the data set which can be movie review dataset, twitter
dataset, etc. These data sets are freely available on internet. Then we preprocess the data set
and prepare a training set for our classifier. Using training set we train the classifier, after
training we provide test data set to classifier.



Natural Language Processing  Approach
================================

Natural Language Processing approach uses SentiWordNet lexicon, which consists of
positive, negative score for each of the term occuring in WordNet. The implementation is
done by extracting the adjectives out of the sentence and then searching it in the
SentiWordNet to find out its positive, negative score. In this way the total net score of the
sentence is calculated and whichever is greater (either positive or negative) becomes the
review for the sentence.


Twitter API v1.1. is used in get_twitter_data.py  
Add the consumer_key, consumer_secret, access_token, access_oken_secret in config.json file or pass it via command line. 
Try test_twitter_data.py for a sample example.
