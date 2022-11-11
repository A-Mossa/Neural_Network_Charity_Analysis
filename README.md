# Neural_Network_Charity_Analysis

## Overview of the project

Utilizing Neural Network Machine Learning model to facilitate the prediction of new applicantions, and determine the potential success when Alphabet Soup funding is granted. 
The dataset used contatined information about application type, classification, field, status, current income, and if the specific application was successful or not.

## Results

### Data Preprocessing

![PreProcessing](https://github.com/A-Mossa/Neural_Network_Charity_Analysis/blob/main/Imgs/PreprocessingDF.png)

- What variable(s) are considered the target(s) for your model?
  - "IS_SUCCESSFUL" parameter was selected as the target as it is a statement of the success or the failure of the application.
  
- What variable(s) are considered to be the features for your model?
  - "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE CASE", "ORGANIZATION, STATUS", "INCOME_AMT", "SPECIAL CONSIDERATIONS", and "ASK_AMT" were the ones selected as features, as they have the most meaningful effect on the project.
  
- What variable(s) are neither targets nor features, and should be removed from the input data?
  - "EIN", and "NAME" were dropped off the model as they pose no real life effect on the success or failure of the project.

### Compiling, Training, and Evaluating the Model

![Model Evaluation](https://github.com/A-Mossa/Neural_Network_Charity_Analysis/blob/main/Imgs/modelEvalDel2.png)

- How many neurons, layers, and activation functions did you select for your neural network model, and why?
  - The model consisted of 1 Input layer, 2 hidden layers, and 1 output layer.
  - Neurons for the first hidden layer are 80 as this simulates almost double the input , and 30 for the second hidden layer which is around the same as the number of inputs.
  - 'Relu' is the function of choice for the 2 hidden layers, on top of a sigmoid function.

- Were you able to achieve the target model performance?
  - No is the answer to that question. the model only slightly came short of the target 75% accuracy score intended.

- What steps did you take to try and increase model performance?
  - the column "ASK_EMT" showed great variance which is not desirable for this ML project. Bucketing was considered, but dropping both this column and the "STATUS" column was the final decision. Adding more neurons to the hidden layer was the next logical step to improve the accuracy and reduce the loss in the model. following that step, an attempt to increase the number of layers were implemented which didnt increase the accuracy score. the final attempt at optimizing the model was the introduction of a different activation function, (tanh), which insignificatly impacted the results .

## Summary

The Neural Network ML model used failed to achieve target of 75% accuracy, and came with a staggering 50% loss, even with optimization. Based on these results the performance of this model wasn't optimal.
Since we are dealing with a classification issue, a supervised ML model such as RandomForest would have better served the purposes of this project at less resource cost.
