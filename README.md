# Classifying Emails as Ham & Spam Using Machine Learning Techniques

The provided dataset is the collection of spam and non-spam emails which is collected from the Enron Coorporation emails available on the web.
The dataset is the text data which contains two folders of spam and ham(non-spam) emails such that 1500 files are collection of spam emails and 3672 of ham emails.
The main motive of this project is to classify the spam or non-spam emails using machine learning algorithms which includes the supervised classification models.
<br><br>
Introduction<br>
The dataset that we will use for this assignment is the Enron email dataset. You can find the
full dataset on the web here: http://www.aueb.gr/users/ion/data/enron-spam/. The dataset is a
collection of public domain emails from the Enron corporation. The emails have been manually
classified as spam and non-spam. The primary goal of the assignment is to create a supervised
classification pipeline to classify emails as spam or non-spam from the training data. You are
free to use either the preprocessed emails or the raw emails for your analysis.
<br><br>Preprocessing<br>
The first stage in the pipeline is to preprocess and clean the dataset.
<br><br>Training and test splits
<br>The very first thing that you will need to do is split the data into training and test sets. Write a
Python script to perform the split: 70% of the data for training and the remainder for test. Take
appropriate measures to ensure that the test set is not biased in any way. There may be duplicate
and empty emails that need to be handled appropriately. Store the resulting training and test
sets in files using any convenient data format that you like. Collect and record statistics on the
resulting training and test sets including total numbers of spam and non-spam emails in each
set.
<br><br>Feature extraction
<br>The second part of preprocessing will be to extract the features you will need for the remainder
of the analysis. You may revisit this stage many times as you become more familiar with the
dataset and the kinds of features that may be useful for the classification task. You may want
to start with using a bag-of-words model here to transform the documents into a fixed length
representation suitable for classification. The sklearn.feature_extraction.text package may be
useful here.
<br>The features you choose will affect the performance of the final classifier, and there are many
possibilities (e.g. stop word removal, TF-IDF encoding, infrequent word removal, etc.). Choose
something you think is reasonable to start with and later you can experiment with alternatives
on the validation set.
<br><br>Exploratory data analysis
<br>Use the training section of the dataset to perform some exploratory data analysis. The goal at
this stage is to become accustomed with the data and gain insights into the kinds of features
may be useful for classification.
<br><br>Explorations Done
<br>Find the top-20 most frequently used words in spam and non-spam emails and use a bar plot
to show their relative frequencies. Compare the distribution of email lengths in spam and non-

<br><br>Supervised classification
<br>Train a supervised classification model on your features and calculate validation accuracy
either on a hold out validation set or using cross validation. Record the final accuracy of the
classifier. How many of the emails are correctly classified by the model? How many are
misclassified? Use the sklearn.metrics package to investigate the kinds of errors that are being
made. Document all findings. Use the Python pickle module to save the model to the disk.
<br><br>Model selection
<br>Select several candidate models that you want to compare. This could include different
classifiers (e.g. naive Bayes MultinomialNB), different hyperparameters, or different sets of
features (remember, hyperparameter selection is part of model selection!). Use a validation set
or cross-validation to compare the accuracy of different models. Create plots to compare a
subset of the models that you investigated during model selection. Retain the most effective
model for evaluation.
<br><br>Model evaluation
Estimate the out-of-sample error for the model that you found to be most accurate during model
selection by evaluating it on the held-out test set. Use the sklearn.metrics package to benchmark
the model in several ways. Create an graph plot for the model. Compute the model's accuracy
on the test set. Comment on the implications of the resulting for a real production classifier.
