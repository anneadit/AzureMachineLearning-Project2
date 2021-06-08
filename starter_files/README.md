

# Operationalizing Machine Learning with Azure

In this project we first configure an Auto ML experiment in Azure ML Studio on a bank marketing dataset with the aim of predicting if a certain individual will make a term deposit. After the experiment has been completed, we deploy the best performing model to an Azure Container Instance and then consume the endpoint with a json payload. Afterwards, we create a automated pipeline using Azure SDK to do develop the same AutoML model, publish it, and then consume it.

## Architectural Diagram

The project consists of the following steps:

Authentication: 
We need to authenticate our credentials and what we are allowed to do with Azure ML. This is automatically taken care of through the Udacity subscription.

Automated ML Experiment:
We run a classification AutoML experiment on the Bank Marketing dataset and then retrieve the best performing model

Deploy the best model
We deploy the best performing model on an Azure Container Instance with authentication enabled.

Enable logging
We enable Application Insights for detailed logging and debugging purposes.

Swagger Documentation
We create a Swagger UI to document our endpoint API in order to make it easier for users to understand the various http requests.

Consume model endpoints
We consume the model endpoint with a JSON payload

Create and publish a pipeline
We automate the aforementioned steps by creating and publishing an AutoML pipeline.

Documentation
Everything is documented in a readme file.

![image](https://user-images.githubusercontent.com/38438203/121116307-4f30c800-c7e4-11eb-92e3-8078b006f251.png)

## Key Steps
*TODO*: Write a short discription of the key steps. Remeber to include all the screencasts required to demonstrate key steps. 

*TODO* Remeber to provide screenshots of the `RunDetails` widget as well as a screenshot of the best model trained with it's parameters.

## Screen Recording
*TODO* Provide a link to a screen recording of the project in action. Remember that the screencast should demonstrate:

## Standout Suggestions
*TODO (Optional):* This is where you can provide information about any standout suggestions that you have attempted.
