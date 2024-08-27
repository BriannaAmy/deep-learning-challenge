# Module 20 Credit Risk Analysis

## Overview of the Analysis

The purpose of the analysis is to build a neural network model that can predict, with an accuracy above 75%, whether or not applicants will be successful if they are funded by Alphabet Soup.

## Results

* Data Processing:

![Screenshot 2024-08-25 194209](https://github.com/user-attachments/assets/14703620-9ddf-40f9-b3c0-b1b09f2ae31c)

  * What variable(s) are the target(s) for your model?
    * The IS_SUCCESSFUL variable is the target for the model.
  * What variable(s) are the features for your model?
    * The included variables used as the features are APPLICATION_TYPE, APPLICATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.
  * What variable(s) should be removed from the input data because they are neither targets nor features?
    * The EIN and NAME variables were removed.

![image](https://github.com/user-attachments/assets/54538343-67e6-411a-a4a2-8b29233614ea)

* Compiling, Training, and Evaluating the Model:
  * How many neurons, layers, and activation functions did you select for your neural network model, and why?
    * After converting the categorical data to numberic and extracting the features, there are a total of 43 neurons for this neural network model. I used a total of two hidden layers that used the Rectified Linear Unit (ReLU) activation function for all of the hidden layers. I used the ReLU activation function as that is most commonly used. I used the sigmoid activation function for the output layer because this is a binary output model. The first hidden layer has 20 nodes, and the second hidden layer has 10 nodes.

![image](https://github.com/user-attachments/assets/086b1cdb-ce3f-4d18-9bfa-2022b91bde2a)
  * Were you able to achieve the target model performance?
    * I was not able to achieve the target model performance with a result of 72.6% accuracy and 55.7% loss.

![image](https://github.com/user-attachments/assets/6addf16a-cd2f-40a5-bdbc-f208ce101fe8)
  * What steps did you take in your attempts to increase model performance?
    * I changed the number of hidden layers, increased the number of nodes for each of those layers, and increased the number of epochs in my attempts to optomize the model.  On my fourth attempt to optimize the model, I changed the activation function used for the hidden layers to hyperbolic tangent (tanh).

![image](https://github.com/user-attachments/assets/1883880e-fa75-4d01-aab9-a8dc8bd0056e)

## Summary

To summarize, all four attempts to create a model with an accuracy above 75% failed.  The accuracy and loss percentages of all models stayed close to the original results of approximately 73% and 56% respectively.

A random forest model might be a better fit because random forest models are very good at handling complex datasets and mitigating overfitting.
