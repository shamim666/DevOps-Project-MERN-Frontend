# repository name: DevOps-Project-MERN-Frontend
# main task: SetUP a complete CICD pipeline of a MERN application on AZURE DevOps

STEPS:
===========  making of azure devops platform ================  
create an organisation under Azure DevOps(dev.azure.com).
create a project under that organisation.There can be multiple projects under one organisation. 
request to microsoft for an agent to run the cicd pipeline for your project under the created organisation. 
requested agent works for all projects under one organisation and the mail will be like below format.
---------------------------------------------------------------------------------------
# To: azpipelines-freetier@microsoft.com <azpipelines-freetier@microsoft.com>
# Hi Team,

# Can you please provide me access to free parallelism grant.

# My name: Shamim Hasan
# My organization name: https://dev.azure.com/shamim666

# Thanks and Regards
# Shamim Hasan 
-----------------------------------------------------------------------------------------
Here above in https://dev.azure.com/shamim666  ,, shamim666 is the created organisation in dev.azure.com

========== creation of cosmos DB ==========
create a cosmos DB 
connect the DB link to the backend code(db.js) and test it by running (node server.js) command

======== back end CICD =========
create repos for backend and front end in azure repos
push backend code (node) to azure repos
create CI pipeline for your backend
After CI build the generated artifact release will be deployed into azure app service
create azure app service in portal.azure.com
create CD pipeline for your backend
connect the azure cosmos DB link to the front end code where the API are being used

========= front end CICD ===========
push the front end code to azure repos
create CI pipeline for your frontend
After CI build the generated artifact release will be deployed into azure storage account
create a storage which contains containers and under container create a container 
create CD pipeline for your front end
then go to index.html file and copy the url and paste it to the browser
thats the full deployed MERN application

=================== Auto Commit Pipeline ============

Now if any body do any changes in frontend or backend code ,  it will automatically test , build , and deployed. 
Thats it.







