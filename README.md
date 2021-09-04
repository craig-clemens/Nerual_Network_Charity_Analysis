# Nerual Network Charity Analysis

## Overview
This project was tasked with using deep-learning neural networks. Utilizing Tensorflow in Python we analized and classified the success (or lack thereof) of charitable donations.

Our methodology included the following:
* preprocessing data for neural networks;
* compile, train and evaluate model;
* attempt to optimize the model.

## Results
### Preprocessing
* Cleaned up input data by removing columns "EIN" and "NAME"
* The column "IS_SUCESSFUL" which contains binary data is the target for our deep learning neural network as it referes to if the charity donation was used effectively.
* Columns "APPLICAITON_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", "ASK_AMT" are collectively the features of our model

We then encoded the categorical variables, split them inot training and testing datasets and applied standardization to our features.

### Compile, Train and Evaluate our Model
Our inital model of two hidden layers with a ReLU activation function and an output binary classifcation, Sigmoid. We used the optimizer adam and the loss function binary_crossetntropy.

With the parameters above the accuracy remained well under 75%. An underwhelming performance. To attempt to increase the accuracy we increased the number of neurons, layers, and tried a different activation function (tanh), however none of these seemed to significantly improve the models performance.

## Summary
Our deep learning neural network model did not reach the 75% target accuracy - overall the performance of this model is certainly not outperforming. As a potential improvement we could utilize a supervised machine learning model like Random Forest Classifier to combine many of the decicions trees to generate a classified output. We could use this to evaluate its performance against our deep learning model.
 
