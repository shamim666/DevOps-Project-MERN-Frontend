# SetUP a complete CICD pipeline of a MERN application on AZURE DevOps

# STEPS:
===========  making of azure devops platform ================  
1. create an organisation under Azure DevOps(dev.azure.com).
2. create a project under that organisation.There can be multiple projects under one organisation. 
3. request to microsoft for an agent to run the cicd pipeline for your project under the created organisation. 
4. requested agent works for all projects under one organisation and the mail will be like below format.

 
 ==== Email Format =========
 
 To: azpipelines-freetier@microsoft.com <azpipelines-freetier@microsoft.com>
 Hi Team,

 Can you please provide me access to free parallelism grant.

 My name: Shamim Hasan
 My organization name: https://dev.azure.com/shamim666



Here above in https://dev.azure.com/shamim666  ,, shamim666 is the created organisation in dev.azure.com

========== creation of cosmos DB ==========
1. create a cosmos DB 
2. connect the DB link to the backend code(db.js) and test it by running (node server.js) command

======== back end CICD =========
1. create repos for backend and front end in azure repos
2. push backend code (node) to azure repos
3. create CI pipeline for your backend
4. After CI build the generated artifact release will be deployed into azure app service
5. create azure app service in portal.azure.com
6. create CD pipeline for your backend
7. connect the azure cosmos DB link to the front end code where the API are being used

========= front end CICD ===========
1. push the front end code to azure repos
2. create CI pipeline for your frontend
3. After CI build the generated artifact release will be deployed into azure storage account
4. create a storage which contains containers and under container create a container 
5. create CD pipeline for your front end
6. then go to index.html file and copy the url and paste it to the browser
7. thats the full deployed MERN application

=================== Auto Commit Pipeline ============

Now if any body do any changes in frontend or backend code ,  it will automatically test , build , and deployed. 
Thats it.







