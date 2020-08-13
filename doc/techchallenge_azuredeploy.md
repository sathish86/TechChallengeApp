## Pre requisites

Need to have below tools and cloud access to deploy the application
  - Azure Devops Access
  - Docker Hub Access
  - Azure Cloud Subsciption

## High Level Architecture

![alt text](https://github.com/sathish86/TechChallengeApp/tree/develop/doc/AzureDeployTechChallenge.png)

## Steps to provision and deploy the solution

- Access [Github Repo](https://github.com/sathish86/TechChallengeApp)
    - Make changes on develop or feature/** branch which will trigger the Azure devops pipeline DEV-TechChallenge to deploy infrastructure and application to Azure cloud in Dev environment.

    - Once changes are satisfactory then create PR from develop and rebase-merge to Master branch which will trigger the Azure devops pipeline PROD-TechChallenge to deploy infrastructure and application to Azure cloud in UAT and PROD environment.
  
- [Access Azure Devops Pipeline](https://dev.azure.com/serviantech/techchallenge/_build) which has both development and production deployment pipeline 

- [Docker Hub](https://hub.docker.com/r/sathish86/techchallengeapp/tags) to check the latest image once the build is complete

- Azure Cloud Subsciption App Service
    - [Development environment App Service ](https://servian-techchallenge-dev.azurewebsites.net/) to check the latest application

    - [UAT environment App Service ](https://servian-techchallenge-uat.azurewebsites.net/) to check the latest application

    - [PROD environment App Service ](https://servian-techchallenge-prod.azurewebsites.net/) to check the latest application