# Alphabet Soup Deep Learning Model for Funding Success Prediction

## Overview of the Analysis

The purpose of this analysis is to create a binary classification model using deep learning techniques to predict if an organization funded by Alphabet Soup will be successful in their venture. The model utilizes a dataset of over 34,000 organizations that have received funding from Alphabet Soup, containing metadata about each organization.


## Results

### Data Preprocessing

- **Target variable(s) for the model:** The target variable for the model is `IS_SUCCESSFUL`.
- **Feature variable(s) for the model:** The feature variables for the model include `APPLICATION_TYPE`, `AFFILIATION`, `CLASSIFICATION`, `USE_CASE`, `ORGANIZATION`, `STATUS`, `INCOME_AMT`, `SPECIAL_CONSIDERATIONS`, and `ASK_AMT`.
- **Variable(s) removed from the input data:** The `EIN` and `NAME` columns were removed from the input data as they are identification columns and not useful as features or targets.


### Compiling, Training, and Evaluating the Model

- **Neurons, layers, and activation functions selected for the neural network model and rationale:** The model consists of three hidden layers with 14, 7, and 4 neurons, respectively, and ReLU activation functions. The output layer uses a sigmoid activation function for binary classification. The structure was chosen to provide a balance between complexity and the potential for overfitting, while maintaining the ability to learn complex patterns in the data.

- **Achievement of the target model performance:** The model did not achieve the target performance of 75% accuracy. However, multiple attempts were made to optimize the model, including adjusting input data, modifying the structure of the neural network, and modifying the training regimen.

- **Steps taken in attempts to increase model performance:** To increase model performance, the following steps were taken:

  - Dropping additional irrelevant columns from the input data.
  - Creating more bins for rare occurrences in columns and adjusting the number of values for each bin.
  - Adding more neurons to a hidden layer.
  - Adding or removing hidden layers.
  - Using different activation functions for the hidden layers.
  - Increasing or decreasing the number of epochs in the training regimen.



## Summary

The deep learning model did not achieve the desired performance of 75% accuracy in predicting the success of Alphabet Soup-funded organizations. However, several attempts were made to optimize the model through data preprocessing and neural network structure adjustments.

As an alternative recommendation, a Random Forest Classifier or a Gradient Boosting Classifier could be used to solve this classification problem. These ensemble learning methods have the potential to provide better accuracy and generalization without being as prone to overfitting as deep learning models. Further exploration of these alternative models may lead to improved performance in predicting the success of funded organizations.

