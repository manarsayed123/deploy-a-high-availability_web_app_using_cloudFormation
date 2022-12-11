# Project2 deploy-a-high-availability-web-app-using-CloudFormation


> In this project (Udagram App), I deployed web servers for a highly available web app using CloudFormation.
> I have created the script that deploys the infrastructure and Servers used for The Udagram app.

## Project Files:
```sh
1- create.sh : Cloudformation create stack script. 
2- update.sh : Cloudformation update stack script.
3- ourinfra.yml : Udagram Project's CloudFormation script.
4- ourinfra-params.json : Udagram Project's CloudFormation script parameters.
5- A Diagram for infrastructure and Servers
```
## Instruction of deploy:
Just run;
```sh
> ./create.sh ourinfraServer ourinfra.yml ourinfra-params.json
```aws cloudformation create-stack --stack-name udagramApp --template-body file://ourinfra.yml --parameters file://ourinfra-params.json --capabilities CAPABILITY_NAMED_IAM
> ./update.sh ourinfraServer ourinfra.yml ourinfra-params.json
```aws cloudformation update-stack --stack-name udagramApp --template-body file://ourinfra.yml --parameters file://ourinfra-params.json --capabilities CAPABILITY_NAMED_IAM
