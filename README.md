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

# Steps and Project Execution Screenshot

# Step 1: Authentication
I used the lab Udacity provided to us, so I skipped this step since I'm not authorized to create a security principal.

# Step 2: Automated ML Experiment

In this step, we first upload our dataset using the dataset's URI:
In this step, I created an AutoML experiment to run using the Bank Marketing Dataset which was loaded in the Azure Workspace, choosing 'y' as the target column.

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

Figure 7: Best Model Selected

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/7.BestModelSelected1.PNG)


Figure 8: Deploy The Model Using ACI

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/8.DeployTheModelUsingACI.PNG)

Figure 9: Deploying Best Model

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/9.DeployingBestModel.PNG)

# Step 4: Enable Application Insights & Logs

Figure 10: Application Insight Enabled

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/10.ApplicationInsightEnabled.PNG)

Figure 11: Deployment Logs

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/11.DeploymentLogs.PNG)

# Step 5: Swagger Documentation

Figure 12: Swagger

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/12.Swagger.PNG)

Figure 13: Swagger


![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/13.Swagger.PNG)


# Step 6: Consume Model Endpoints

Figure 14: Output

![alt text](https://github.com/RajanKumarYadav/Automated-Machine-Learning-on-Microsoft-Azure/blob/main/Screenshoot/14.Output.PNG)

# Step 7: Create, Publish and Consume a Pipeline

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

We can increase the Exit Criterion time from 1 hour to the default value of 3 hours to be able to find models of higher accuracy.
We can enable Data drift tracking to ensure accuracy of the model.
