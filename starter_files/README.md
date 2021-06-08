

# Operationalizing Machine Learning with Azure

In this project we first configure an Auto ML experiment in Azure ML Studio on a bank marketing dataset with the aim of predicting if a certain individual will make a term deposit. After the experiment has been completed, we deploy the best performing model to an Azure Container Instance and then consume the endpoint with a json payload. Afterwards, we create a automated pipeline using Azure SDK to do develop the same AutoML model, publish it, and then consume it.

## Architectural Diagram

### The project consists of the following steps:

### Authentication: 
We need to authenticate our credentials and what we are allowed to do with Azure ML. This is automatically taken care of through the Udacity subscription.

### Automated ML Experiment:
We run a classification AutoML experiment on the Bank Marketing dataset and then retrieve the best performing model

### Deploy the best model
We deploy the best performing model on an Azure Container Instance with authentication enabled.

### Enable logging
We enable Application Insights for detailed logging and debugging purposes.

### Swagger Documentation
We create a Swagger UI to document our endpoint API in order to make it easier for users to understand the various http requests.

### Consume model endpoints
We consume the model endpoint with a JSON payload

### Create and publish a pipeline
We automate the aforementioned steps by creating and publishing an AutoML pipeline.

### Documentation
Everything is documented in a readme file.

### Architecture Diagram
![image](https://user-images.githubusercontent.com/38438203/121116307-4f30c800-c7e4-11eb-92e3-8078b006f251.png)

## Key Steps

### Automated ML Experiment

  1. We use the registered bank marketing dataset
  ![image](https://user-images.githubusercontent.com/38438203/121117947-fc0c4480-c7e6-11eb-8f75-12b5edde0203.png)
  
  2. Run the classification AutoML Experiment
  ![image](https://user-images.githubusercontent.com/38438203/121118109-4988b180-c7e7-11eb-89ab-742c740db86d.png)

  3. Retrieve the best performing model which is a Voting Ensemble model
  ![image](https://user-images.githubusercontent.com/38438203/121118210-76d55f80-c7e7-11eb-89a6-e992cb8b07b8.png)
  
  ![image](https://user-images.githubusercontent.com/38438203/121118245-83f24e80-c7e7-11eb-9076-d0035c3a408f.png)
  
### Deploy the best performing model

  1. We deploy the best performing model on an Azure Container Instance with authentication enabled
  ![image](https://user-images.githubusercontent.com/38438203/121118620-2b6f8100-c7e8-11eb-8d9b-ff3012c8806f.png)

### Enable Logging

  1. We enable logging for the deployed model in Azure SDK using the logs.py script
  ![image](https://user-images.githubusercontent.com/38438203/121118826-85704680-c7e8-11eb-81ef-0b716ca40902.png)



  



*TODO* Remeber to provide screenshots of the `RunDetails` widget as well as a screenshot of the best model trained with it's parameters.

## Screen Recording
*TODO* Provide a link to a screen recording of the project in action. Remember that the screencast should demonstrate:

## Standout Suggestions
*TODO (Optional):* This is where you can provide information about any standout suggestions that you have attempted.
