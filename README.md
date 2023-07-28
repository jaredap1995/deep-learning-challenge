# Module 12 Deep Learning Report

## Overview of the Analysis

The aim of this analysis was to utilize a deep learning model, specifically a neural network, to predict if an organization funded by Alphabet Soup will be successful. The success of an organization was determined based on various features present in the dataset.

## Results

### Data Preprocessing

* The target variable for the model was the success of the organization, i.e., whether the organization will be successful or not.
* The features for the model included all other variables in the dataset excluding the target variable and the variables that were neither targets nor features.
* The `EIN` and `NAME` columns were removed from the input data, as they were neither targets nor features, simply identifiers not relevant to the prediction model.

### Compiling, Training, and Evaluating the Model

The neural network model comprised of 3 Dense layers of 80,30, and 1 neuron respectively. 

For a binary classification problem like this, the output layer contained a sigmoid activation function. The number of neurons in the hidden layers often depends on the number of input features, with various strategies such as taking the average of the input and output neurons.

Achieving the target model performance was unfortunately not possible, the model continued to get stuck in gradient descent despite multiple attmepts to change the data and features including:

* Dropping columns, handling outliers, and changing the way we bin rare occurrences in columns.
* Modify the network architecture, added and removed layers and optimizers etc.
* Changing the epochs and batch_size

## Summary

In summary, the deep learning model was developed to predict the success of organizations funded by Alphabet Soup. This involved a process of data preprocessing, model compiling and training, and model evaluation. If the target predictive accuracy of over 75% was not achieved, various optimization steps were taken to try and improve the model performance to no avail. 

For future work, I would recommend using ensemble machine learning models such as Random Forest or Gradient Boosting. These models can often perform well on a wide range of datasets and might provide a useful comparison to the performance of the deep learning model. Ensemble models work by creating multiple models (or "weak learners") and combining their predictions, which often results in more robust and accurate predictions. It would be interesting to compare the performance of these traditional machine learning models with the deep learning model used in this analysis.
