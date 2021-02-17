# CI-CD-serverless
Build Python CI/CD in Azure DevOps and deploy to Azure Functions and AWS lambda 

Create a Build Pipeline

Let’s start a pipeline by selecting a source and repository branch and by selecting a classic editor.

![image](https://user-images.githubusercontent.com/58148717/108228282-541e1e80-7104-11eb-8094-20daacda9b4a.png)

![image](https://user-images.githubusercontent.com/58148717/108228322-5d0ef000-7104-11eb-9e73-747435312c95.png)

Once you click on the button Apply you can see the next screen with all these tasks. 

You can change the pipeline name as you want. 

If you notice the tasks it is using the Python version 3.6, install dependencies, tuns build script, archive files, and publish the artifact and for AWS deploy to lambda

Let’s build the pipeline manually this time by clicking on the Queue.

We could also create CI for lambda function as well first you need to create lambda function in AWS and then either create a AWS service connection in Azure devops or create variables in build pipeline make sure to get AWS tool kit for Azure DevOps from market place. 

https://marketplace.visualstudio.com/items?itemName=AmazonWebServices.aws-vsts-tools

Once ready add template deploy to Lambda in the last

![image](https://user-images.githubusercontent.com/58148717/108228790-cf7fd000-7104-11eb-80cb-52062d459c03.png)

Release pipeline for Azure Functions.

![image](https://user-images.githubusercontent.com/58148717/108228896-e3c3cd00-7104-11eb-996d-edf82f76db44.png)

Once validation/authorizations are done save the release and it will trigger. 

I have also attached the complete YAML file. 







