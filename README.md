# ARM-Template-Deployment-with-Azure-Pipeline
This project is aimed at creation and deployment of Azure resources using ARM template. The resources are provisioned as infrastructure as code (IaC) with ARM template and deployed in a CI/CD approach with azure DevOps pipeline. Azure resources to be created are App service plan and App service.

**Steps**
1. The ARM template code is developed as json file titled tomapp.json with the azure services to be created defined as 'resources'. the basic properties of the resources are defined in the code. this code creates the App service plan and the App service. unique properties of the App service such as the name, SKU, and location are specified in the parameters file (tommapp.parameters.json).
2. a local repository in VScode and remote in Azure DevOps are created using the git commands.
3. a yaml file is define with code to enable the deployment of the asure resources from the azure pipeline. to enable thuis peipleine to run and access the azure portal and resources, appriopriate connections are enable with permission.
4. the pipeline is run to create the app service plan and app service.
5. another peipleine is created to build and deploy a dot net web application to the created app service.

<img width="1439" alt="image" src="https://github.com/thompsonanigbo/ARM-Template-Deployment-with-Azure-Pipeline/assets/103883140/26a145c2-9f6e-476a-8bd6-ea598725f257">

