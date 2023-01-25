# azure-sql-deployment-simplifiedYAML
Deploy just a database using Yaml

## Start a Visual Studio Database Project
Create a database project in Visual studio. I built an Azure database, so make sure to go to properties and set the database as an azure database and not SQL server 2016 or anything. 

Make a few tables and views, and procedures, whatever you want.  Make sure it builds properly in the Visual Studio IDE. 
Save your project to your git repository like I have. See the only folder in this repo, it contains the Database project. 

# Become a YAML hero
## Build the database

Start with a Stage yaml file. This will call both your build and your deploy jobs. 
They have to be separate because the job after the build does a pre deploy, and you first need to build the dacpac and then go and fetch it with a pre deploy


