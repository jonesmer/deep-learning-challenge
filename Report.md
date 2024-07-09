# Analysis Report
Funding Applicant Success Model
## Overview
The purpose of this analysis is to use historical data to predict success with Alphabet Soup funding. We used a neural network to model the data.
## Results
### Data Preprocessing
The data used includes many fields - most of which are useful for the model.
* The target variable is IS_SUCCESSFUL - this indicates whether funding was used effectively.
* The features include industry sector affiliation, government organization classification, use case for the funding, organization type, active status, income classification, special considerations, and the amount requested.
    - Some of these features had a large number of unique values. To help with the analysis, the more rare types were all added into an "Other" bucket.
* EIN and name were also included in the data; these are not useful in the analysis so they were removed.
### Compiling, Training, and Evaluating the Model
* In the first model, we used 2 layers and 111 nodes (80 in Layer 1, 30 in Layer 2, 1 for the output). We used a relu activation function in the hidden layer and a sigmoid activation function in the output layer.
* A second model was created - this one included more condensed data (income classifications were condensed further to decrease the number of columns in the data), more epochs, and more nodes in the second layer.
## Summary
The goal for these models is 75% accuracy.
* The first model had an accuracy of 72.86%.
* The second model had an accuracy of 72.72% - no improvement from the first model.
* Things that could improve the model further include:
    * more layers or more nodes
    * different activation functions
    * further data preprocessing/condensing.

Another model could solve this classification problem if these things were taken into consideration.