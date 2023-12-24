Deep Learning Finds "Fake News" with 97% Accuracy
In his article published on KDnuggets in 2017 George McIntire describes an experiment building a "fake news" classifier using a document-
vector model and Naive Bayes approach. He reports an 88% accuracy when classifying a "fake news" dataset which he assembled from various
sources. This of course immediately made me wonder if deep neural networks (DNNs) can do better and if the performance increase due to
these deep learners is statistically significant compared to the performance of the Naive Bayes classifier.
The Original Experiment
In the original experiment McIntire constructed a Naive Bayes classifier to classify the articles in his dataset as "Real" or "Fake" news. As
published on GitHub the McIntire's "fake news" dataset has 6335 news articles of which 3171 articles are "real news" and 3164 articles are "fake
news". The dataset is well balanced with respect to the two classes.
Note: The dataset as published contains a few more articles but the 'text' field for those articles is empty. These articles were removed for
the analysis here.
I recreated McIntire's experiment using the following,
