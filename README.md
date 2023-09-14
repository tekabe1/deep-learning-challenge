# deep-learning-challenge

Analysis Report: Predicting Charitable Organization Success with a Neural Network

Overview

The objective of this analysis is to develop a predictive model using a deep learning neural network to classify charitable organizations funded by Alphabet Soup as either "successful" or "unsuccessful". The model aims to provide Alphabet Soup with a tool for making more informed decisions regarding which organizations to fund.

Data Preprocessing

Target and Features
Target Variable: The target variable is IS_SUCCESSFUL, indicating whether an organization is successful (1) or not (0).
Features: The model uses features including APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, and SPECIAL_CONSIDERATIONS.
Removed Variables: The EIN and NAME columns were removed as they don't contribute to the predictive power of the model.

Compiling, Training, and Evaluating the Model

Model Architecture
Input Features: 117
Hidden Layers: 2
Nodes in Hidden Layers: 80 (1st layer), 30 (2nd layer)
Activation Functions: ReLU (hidden layers), Sigmoid (output layer)

Model Performance
Accuracy on Test Data: 73.11%

Results
Were you able to achieve the target model performance?

The model achieved an accuracy of approximately 73.11% on the test data, meeting our target performance.
What steps did you take in your attempts to increase model performance?

I employed feature engineering, standardization, and experimented with different model architectures to find the optimal balance.

What variable(s) are the target(s) for your model?
The target variable for the model is IS_SUCCESSFUL.

What variable(s) are the features for your model?
The features for the model include attributes like APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, and SPECIAL_CONSIDERATIONS.

What variable(s) should be removed from the input data because they are neither targets nor features?
The EIN (Employer Identification Number) and NAME columns were removed.

How could you use a different model to solve the same problem, and why?
An ensemble method like Random Forest or Gradient Boosting could be used. They are often more interpretable, require less fine-tuning, and can handle a larger number of features effectively. The choice depends on interpretability, computational resources, and dataset characteristics.

Summary

The neural network model demonstrated reasonable performance in classifying charitable organizations. With an accuracy of 73.11%, the model shows promise. However, considering factors like interpretability and computational resources, exploring ensemble methods may be beneficial. Both approaches should be further evaluated to determine the most suitable solution for Alphabet Soup's specific needs.

Recommendations

It is recommended to further evaluate both the neural network model and ensemble methods, possibly consulting with domain experts. Additionally, a broader exploration of model architectures and hyperparameters may lead to further improvements in predictive accuracy.
