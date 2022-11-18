## Exersices for Chapter 02

### 1. 
**Q:** Try to build a classifier for the MNIST dataset that achieves over 97% accuracy on the test set. Hint: the KNeighborsClassifier works quite well for this task; you just need to find good hyperparameter values (try a grid search on the weights and n_neighbors hyperparameters).

### 2.
**Q:** Write a function that can shift an MNIST image in any direction (left, right, up, or down) by one pixel.5 Then, for each image in the training set, create four shifted copies (one per direction) and add them to the training set. Finally, train your best model on this expanded training set and measure its accuracy on the test set. You should observe that your model performs even better now! This technique of artificially growing the training set is called data augmentation or training set expansion.

### 3.
**Q:** Tackle the Titanic dataset. A great place to start is on Kaggle.

### 4.
**Q:** Build a spam classifier (a more challenging exercise):

#### 4.1. 
Download examples of spam and ham from Apache SpamAssassin’s public datasets.

#### 4.2.
Unzip the datasets and familiarize yourself with the data format.

#### 4.3.
Split the datasets into a training set and a test set.

#### 4.4.
Write a data preparation pipeline to convert each email into a feature vector. Your preparation pipeline should transform an email into a (sparse) vector that indicates the presence or absence of each possible word. For example, if all emails only ever contain four words, “Hello,” “how,” “are,” “you,” then the email “Hello you Hello Hello you” would be converted into a vector [1, 0, 0, 1] (meaning [“Hello” is present, “how” is absent, “are” is absent, “you” is present]), or [3, 0, 0, 2] if you prefer to count the number of occurrences of each word.
You may want to add hyperparameters to your preparation pipeline to control whether or not to strip off email headers, convert each email to lowercase, remove punctuation, replace all URLs with “URL,” replace all numbers with “NUMBER,” or even perform stemming (i.e., trim off word endings; there are Python libraries available to do this).
Finally, try out several classifiers and see if you can build a great spam classifier, with both high recall and high precision.