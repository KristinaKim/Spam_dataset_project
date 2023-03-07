# Spam_dataset_project

Problem statement

 The SMS Spam Collection is a set of SMS tagged messages that have been collected for SMS Spam research. It contains one set of SMS messages in English of 5,574 messages. tagged according being ham (legitimate) or spam.
 The files contain one message per line. Each line is composed by two columns: v1 contains the label (ham or spam) and v2 contains the raw text  
1. Perform exploratory data analysis to discover properties of ham/spam mail.
2. Build a model that predicts whether a message is ham/spam.

In this project, we tried worked with NLP and built a model for predicting ham or spam.
* Before transforming a text column using sklearn's CountVectorizer, we eliminated the punctuation, then we split all the words  and made them all lower case. The we found each word root with lemmatizer. CountVectorizer was used for calculating an individual word count in the text.
* Analysis of the dataset showed that the dependent variable is imbalanced (not spam 76.12%, spam 23.88%).
* First, we trained the model using a pipeline with the original dependent variable. Then, we used a combination of oversampling and undersampling methods and balanced the target variable and trained model.
* A total of 16 models were trained (8 models without special balancing and 8 models with a сombination of over- and under-sampling method).
* The model MultinominalNB with Vectorizer showed the best result with 99% accuracy.
* The worst model is KNN with Vectorizer and Balance with an accuracy of 91%.
