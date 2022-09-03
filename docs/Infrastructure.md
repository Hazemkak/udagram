# Infrastructure Description
## RDS:

I used rds postgres first to initialize my database then i copied the credentials of database
to my environment variables in elastic beanstalk to make the api able to connect to the database

## Elastic Beanstalk:

I started first by building the application and zipping it then uploading the zipped version to
elastic beanstalk through CI/CD in CricleCi as well as adding the needed environment variables
using `eb setenv` command

## S3 bucket

I used it to upload my frontend built folder and used the link of the deployed api in it to connect to it correctly.
I used to deploy it to the s3 bucket a bash script found in bin directory

## CircleCI

I used it to make CI/Cd to my project after connecting it to the github repository of the project i made
package.json which include all the scripts i will need in my pipeline & i made 3 jobs :

1. building frontend & backend
2. deploying frontend
3. deploying backend api
