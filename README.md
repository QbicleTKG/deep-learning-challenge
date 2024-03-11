# deep-learning-challenge

During the 2nd iteration of each test, I left the NAME column in, binned the lower-occurring names into Other, and cut out a sample of the data set to make testing run more efficiently.


## Project Overview
The nonprofit foundation Alphabet Soup wanted a tool that can help it select the applicants for funding with the best chance of success in their ventures. Using the Tensorflow neural network library, I used the provided dataset to attempt create an accurate binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

## Dataset

Here is an overview of each data point available in our data set:  

EIN and NAME—Identification columns  
APPLICATION_TYPE—Alphabet Soup application type  
AFFILIATION—Affiliated sector of industry  
CLASSIFICATION—Government organization classification  
USE_CASE—Use case for funding  
ORGANIZATION—Organization type  
STATUS—Active status  
INCOME_AMT—Income classification  
SPECIAL_CONSIDERATIONS—Special considerations for application  
ASK_AMT—Funding amount requested  
IS_SUCCESSFUL—Was the money used effectively  

IS_SUCCESSFUL is our predictor or our ```y``` variable.

This was a very large data set, with a lot of one-off values and classifiers that needed to be binned in order to allow our model to run more efficiently.
![image](https://github.com/QbicleTKG/deep-learning-challenge/assets/139186713/a1197205-dcd9-4c78-96ec-bce7c1726888)
![image](https://github.com/QbicleTKG/deep-learning-challenge/assets/139186713/1a2e43ea-0dbd-4bf2-8ffd-e531f8a2c437)

Here I binned the lesser-occurring application types and classifications to reduce the amount of singular values. This was done consistently on all models.

A different technique I implemented only on the second iteration of each model, was to include the 'NAME' column in the data set, instead of dropping it. Ultimately this led to greater accuracry in my models, but inititally there was FAR too much data for the model to run, and not even Google Collab could run it.

![image](https://github.com/QbicleTKG/deep-learning-challenge/assets/139186713/bce0f719-44b7-4a3a-a71c-04b275c8f517)

To fix this, I binned the NAME values using the same technique as the CLASSIFICATION and APPLICATION_TYPE columns, and captured a random 30% sample for testing, instead of the whole data set. This resulted in much more efficient and timely model fitting and training.

## Model Architecture
I ultimately ran 6 models in an attempt to achieve higher accuracy:
1. Deep Neural Network Model - 72.5% accuracy achieved
2. Deep Neural Network Model w/ NAME column included - 78.8% accuracy achieved
3. Neural Network model implementing hyperparameter keras tuner - 72.3% accuracy achieved
4. Neural Network model implementing hyperparameter keras tuner w/ NAME column included - 78.9% accuracy achieved
5. Neural Network model implementing Bayesian keras tuner - 72.7% accuracy achieved
6. Neural Network model implementing Bayesian keras tuner w/ NAME column included - 78.3% accuracy achieved


## Training Process
- Explain the training process, including the optimization algorithm and hyperparameters used.
- Discuss any data augmentation techniques employed during training.
- Provide details about the training duration and convergence criteria.

## Results and Evaluation
- Present the results obtained from the trained model.
- Discuss the evaluation metrics used to assess the model's performance.
- Compare the model's performance against baseline or state-of-the-art approaches.

## Discussion
- Analyze the results and discuss any insights gained from the project.
- Highlight the strengths and limitations of the approach used.
- Identify potential areas for improvement or future work.

## Conclusion
- Summarize the key findings and contributions of the deep-learning-challenge repository.
- Discuss the implications of the project and its potential applications.

## References
- Include a list of references to any external sources or research papers used in the project.

.
