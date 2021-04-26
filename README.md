# Automated-Machine-Learning-on-Microsoft-Azure-using-MLOps
Automated Machine Learning on Microsoft Azure Cloud with project production, deployment and consumption

Project Overview:
In order to get complete understanding of Azure Cloud with Machine Learning Life Cycle, We need to understand the overall workflow of ML Studio.So we have implemented complete project right from the data upload (Bank Marketing Dataset) to deployment and consumption of endpoints.Also I have implemented complete workflow with Jupyter Notebook to create, publish and consume a pipeline using Python SDK.

Below are the Key Components of Projects:

Microsoft Account Authentication : I am using udacity provided Microsoft Subscription so we dont need this step(You can create security principal if you are using your own Microsoft Account).

Automated ML Experiment : After uploading Bank Marketing dataset, we will configure the AutoML with Compute Cluster, Model training and selecting the model which have higher Accuracy.

Choosing & Deploying the Best Model : When AutoML Experiment will get completed, we will choose best ML model among all the available model based on higher Accuracy.And after that we will deploy that model so all the stake holder of the project can consume the ML Service.

Enable Application Insights & Logs : After choosing & deploying we will do insights for deployed model to monitor the model in real time and check logs of deployed model behaviour.

Swagger Documentation : This section of project will show how to generate swagger document for deployed ML model so that user can run using UI and after this step you will also get JSON object for consuming the model (However you can use any professional API testing tool to test the deployed model ex Postman).

Consume Model Endpoints : Since i am solving binary classification problem i would love to demonstrate you how to get end results.  

Create, Publish and Consume a Pipeline: This step is all about running a Jupyter Notebook to make a pipeline of AutoML which we have already done in previous steps so we can automate the model training & deploymnet of the model comparatavely in no time.

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/azure_automl_architectural_diagram.png)

The overall project goal is to load the data set, configure, deploy, consume any Machine Learning model which is trained using Automated ML and consume the Endpoint. And also we will see the operationalizing ML Model to creating, publishing, and consuming a pipeline.

# Steps and Project Execution Screenshot

# Step 1: Authentication
I am using udacity provided Microsoft Subscription so we do not need this step (You can create security principal if you are using your own Microsoft Account).

# Step 2: Automated ML Experiment

After uploading Bank Marketing dataset, we configured the AutoML with Compute Cluster, trained the model and selected the model, which have higher Accuracy. Since we are going to solve binary classification, we have selected target column as 'y'.

Figure 1: Bank Marketing Dataset

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/1.Dataset.PNG)

I uploaded this dataset into Azure ML Studio in the Registered Dataset Section using the url provided in the project.

For the compute cluster, I used the Standard_DS12_v2 for the Virtual Machine and 1 as the minimum number of nodes.

I ran the experiment using classification, without enabling Deep Learning. The run took some time to test various models and found the best model for the task.

Figure 2: AutoML Run With Registerd DataSet

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/2.AutoMLRunWithRegisterdDataSet.PNG)

Figure 3: Experiment Run Using Classification

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/3.ExperimentRunUsingClassification1.PNG)

Figure 4: Experiment Run Using Classification

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/4.ExperimentRunUsingClassification2.PNG)

Figure 5: Experiment Completed

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/5.ExperimentCompleted.PNG)

Figure 6: Experiment Completed


![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/6.ExperimentCompleted1.PNG)

# Step 3: Choosing & Deploying the Best Model

In this step AutoML Experiment is completed, Now we have choosed best ML model among all the available model based on higher Accuracy.And after that we deployed that model so all the stake holder of the project can consume the ML Service.

Figure 7: Best Model Selected

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/7.BestModelSelected1.PNG)


Figure 8: Deploy The Model Using ACI

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/8.DeployTheModelUsingACI.PNG)

Figure 9: Deploying Best Model

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/9.DeployingBestModel.PNG)

# Step 4: Enable Application Insights & Logs

After choosing & deploying, we have enabled insights for deployed model to monitor the model in real time and check logs of deployed model behavior.

Figure 10: Application Insight Enabled

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/10.ApplicationInsightEnabled.PNG)

Figure 11: Deployment Logs

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/11.DeploymentLogs.PNG)

# Step 5: Swagger Documentation

This section of project will show how to generate swagger document for deployed ML model so that user can run using API UI and after this step you will also get JSON object for consuming the model (However you can use any professional API testing tool to test the deployed model like Postman,etc..).

Figure 12: Swagger

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/12.Swagger.PNG)

Figure 13: Swagger


![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/13.Swagger.PNG)


# Step 6: Consume Model Endpoints

Since i am solving binary classification problem i would love to demonstrate you how to get end results.  

Figure 14: Output

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/14.Output.PNG)

# Step 7: Create, Publish and Consume a Pipeline

This step is all about running a Jupyter Notebook to make a pipeline of AutoML which we have already done in previous steps so we can automate the model training & deployment of the model comparatively in no time.

Figure 15: Running Pipeline

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/15.RunningPipeline.PNG)

Figure 16: Running Pipeline In AzureML

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/16.RunningPipelineInAzureML.PNG)

Figure 17: Pipeline Created

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/17.PipelineCreated.PNG)

Figure 18: Pipeline Endpoint

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/18.PipelineEndpoint.PNG)

Figure 19: Pipeline Run Overview

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/19.PipelineRunOverview.PNG)

Figure 20: Pipeline End Point

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/20.PipelineEndPoint.PNG)

Figure 21: Use Run Details Widget

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/21.UseRunDetailsWidget.PNG)

Figure 22: Schedule Run

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/22.ScheduleRun.PNG)


# Step 8: Demo & Documentation

# Screencast of the Project (Demo)

https://youtu.be/BLOfY19Xb6o

# Future Enhancement of the Project

We can run our custom model to get higher accuracy, In our case we have achieved higher accuracy with Voting Ensemble model If dataset is large we can use optimized XGBoost algorithm after hyperparameter tuning to achieve higher accuracy is less time.
Also in any classification problem there might be class imbalance problem and if you observe the dataset closely you will find class imbalance problem.

And we can use below method to overcome the Class Imbalance Problem
1) Resampling our Dataset
2) By Generating Synthetic Samples
3) Try Different Algorithms
4) Try Penalized Models
5) Use SMOTE (Synthetic Minority Oversampling Technique)

