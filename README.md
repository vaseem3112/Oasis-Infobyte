# Oasis-Infobyte

TASK - Email Spam Detection using Machine Learning

Introduction
In this article, we will explore how to detect email spam using machine learning. Email spam refers to unsolicited and unwanted emails that are sent in bulk to a large number of recipients. By using machine learning algorithms, we can train a model to classify emails as either spam or not spam based on their content.

Key Concepts
To detect email spam, we will use the following key concepts:

Dataset: We will use a dataset that contains a collection of emails labeled as spam or not spam. This dataset will be used to train and test our machine learning model.

Feature Extraction: We will convert the text content of the emails into numerical features that can be used by the machine learning algorithm. In this case, we will use the CountVectorizer class from the scikit-learn library to convert the text into a matrix of token counts.

Training and Testing Sets: We will split the dataset into training and testing sets. The training set will be used to train the machine learning model, while the testing set will be used to evaluate the performance of the model.

Naive Bayes Classifier: We will use the Multinomial Naive Bayes classifier, which is a popular algorithm for text classification tasks. This classifier is based on the Bayes' theorem and assumes that the features are conditionally independent.

Model Evaluation: We will calculate the accuracy of the model by comparing the predicted labels with the actual labels in the testing set.

Code Structure
The code provided follows the following structure:

Load the dataset: The code reads a CSV file containing the email data and stores it in a pandas DataFrame.

Split the dataset: The code splits the dataset into training and testing sets using the train_test_split function from the scikit-learn library. The training set contains 80% of the data, while the testing set contains 20%.

Feature Extraction: The code creates a CountVectorizer object to convert the text content of the emails into numerical features. The fit_transform method is used to fit the vectorizer on the training set and transform the training set into a matrix of token counts. The transform method is used to transform the testing set into the same format.

Train the Classifier: The code creates a Multinomial Naive Bayes classifier object and trains it on the training set using the fit method.

Make Predictions: The code uses the trained classifier to make predictions on the testing set using the predict method.

Model Evaluation: The code calculates the accuracy of the model by comparing the predicted labels with the actual labels in the testing set using the accuracy_score function from the scikit-learn library. The accuracy is then printed to the console.
