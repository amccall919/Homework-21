# Module-21
Deep Learning - Alphabet Soup

## Background

Alphabet Soup, a nonprofit organization, aims to develop a tool that can identify applicants most likely to succeed if awarded funding. By applying machine learning and neural network techniques, I designed a binary classifier to analyze the dataset's features and predict an applicant's success.

The dataset provided by Alphabet Soup contains over 34,000 records of organizations that previously received funding. These records include various metadata about each organization. Using TensorFlow, I built and fine-tuned a deep learning model to predict success. After compiling, training, and evaluating the model, I assessed its loss and accuracy.

## Analysis Overview

The objective of this analysis is to build a predictive model to assist Alphabet Soup in identifying applicants with the highest potential for success.

### Results
Data Preprocessing:

- Target Variable: The target variable for this model is Is-Successful.
- Feature Variables: The input features include name, application type, affiliation, classification, use case, organization, income, special consideration, status, and ask amount.
- Excluded Variables: The EIN (Employer Identification Number) column was removed since it does not contribute to the model’s predictions.

### Model Configuration & Performance
- Neural Network Design: 
 - Architecture: The neural network includes three hidden layers, each with a significant number of neurons to optimize accuracy above 75%.
 - Activation Functions: The first layer uses the relu activation function, while subsequent layers apply the sigmoid function to enhance performance.
- Model Results: The model successfully achieved the target performance, with an accuracy surpassing 75%.
- Transformed the name variable into dummy variables, significantly boosting efficiency despite added computational cost.
- Introduced a third hidden layer using the sigmoid activation function, further improving the model’s predictions.

### Summary
The final model achieved over 75% accuracy, accurately classifying 75% of the test data. Additionally, organizations meeting specific criteria, such as having a name that appears more than five times and using particular application types (e.g., T3, T4, T5), demonstrated an 80% likelihood of success.

### Recommendation
A potential alternative approach could involve using a Random Forest algorithm. This method would divide the dataset into smaller, interpretable decision trees, allowing for improved optimization and potentially more efficient predictions.
