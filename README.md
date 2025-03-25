# Spam Email Classification

This project involved building a machine learning model to classify emails as either spam or legitimate using Naive Bayes. The project started by conducting a data cleaning and exploratory data analysis (EDA). I then measured the performance of the model using metrics like accuracy, precision, recall, F1 score, confusion matrice.

## Why Naive Bayes?
The supervised learning classification algorithm for spam detection that I chose for this was Naive Bayes. Naive Bayes is commonly used in spam filtering. In this case, Naive Bayes would calculate the probability of each class given its data points, and will then choose the class with the highest probability. Naive Bayes is an especially good at text classifications, and can handle the high quantity of text emails can produce, and therefore seems like the correct choice for this task. Specifically the Multinominal Naive Bayes classifier.


## Dataset
https://www.kaggle.com/datasets/balaka18/email-spam-classification-dataset-csv

## Key Features
### Cleaning the Dataset
- Imported and cleaned the dataset by checking for and removing missing values and duplicates.
- Conducted an EDA using descriptive statistics and visualizations to understand the feature distributions and class imbalance.

### Feature Engineering
- Removed non-informative columns like "Email No."
- Defined features (X) and target (y)
- Split the data into training and teseting sets, using an 80/20 split

### Modeling
- Used Multinominal Naive Bayes classifier
- Trained the model on the training set
- Evaluated its performance on the test set

## Model Evaluation
Accuracy: 0.9545893719806763
Precision: 0.890282131661442
Recall: 0.9594594594594594
F1 Score: 0.9235772357723576
<br>
Confusion Matrix:
 [[704  35]
 [ 12 284]]
<br>
### Results:
The results of the metrics show that the model can filter out spam vs. legitimate emails, with an accuracy (number of correct email classifications) of 95.46%, with a precision (percentage of correct spam emails) of 89.03%, a recall (emails counted as spam that were actually spam) of 95.95%, and the F1 Score (a formula that combines the precision and recall with a focus on lower values, meant to indicate if the performance is good or not) of 92.36%, which is closer to 1 and 0 and considered a good overall performance, because it indicates that the model has a good balance of minimizing false positives, and false negatives.

<br>

### Confusion Matrix:
- The top left number (704) is the True Negatives, which are the number of correctly predicted legitimate emails.

- The top right number (35) is the False Positives, which is the number of legitimate emails incorrectly classified as spam.

- The bottom left number (12) is the False Negatives, which is the number of spam emails incorrectly classified as legitimate emails.

- The bottom right number (284) is the True Positives, which is the number of correctly classified spam emails.
