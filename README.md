# DigitRecognizer

## Introduction


This project is for Kaggle’s Digit Recognizer Competition. The goal is to build a model that can correctly identify handwritten digits from the given dataset.

The training set has 785 columns and 42000 rows. Each row stores the data of one handwritten digit, so there are 42000 handwritten digits in total. The first column is the label of the digit, and the rest 784 columns is a flattened 28*28 matrix, which represents a 28 pixels * 28 pixels image. For example, pixel0 is on the first pixel on the first row, and pixel29 is the second pixel on the second row. Each column contains a number from 0 – 255, which indicates the lightness of the pixel. 


## Method

In this project, a K nearest neighbor classifier will be built to identify digits based on their pixels. 

Since the test.csv that Kaggle provides does not contain the correct label for each digit and it is only for submission, it is not used in the training part to validate the accuracy of the model. Instead, the train.csv will be split in to a 75% training set and 25% testing set to evaluate the accuracy of the model. Then the KNN classifier is tuned to find the best value of k. 

