# Automated-Machine-Learning-on-Microsoft-Azure-using-MLOps
Automated Machine Learning on Microsoft Azure Cloud with project production, deployment and consumption

Project Overview: In this project we have used the Bank Marketing Dataset which I have downloaded from the link provided in the project information. In the project I have used Azure to configure a cloud based machine learning production model, deployed it and then consumed it. I have also created, published and consumed a pipeline using Python SDK.

In this project, we'll follow above steps, these are:

Authentication: As we were using udacity workspace so we can't do this step beacuse we are not authorized to create a security principal.

Auto ML model: In this project we will configure the AutoML, train and find the best model.

Deploy the best model: In this step we use best model from step 2 and deploy it so others can use it.

Enable logging: After deploying we'll enable application insights to monitor and check logs of model behaviour.

Documentation: In this step we'll create swagger document for the deployed model so that anyone can run using UI.

Consume model endpoints: In this step we'll write a python script in which we'll use the model endpoint to get inference.

Create and publish a pipeline: In this step we'll create a pipeline of all step (excluding step 4 and 5) and publish it on Azure so that one can use pipeline on new data and run experiment doing manually.

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/azure_automl_architectural_diagram.png)

In this project, we are going to configure, deploy, consume a model which is trained using Automated ML and consume the Endpoint. The Project also involves in creating, publishing, and consuming a pipeline.
