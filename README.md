# CSYE6225-Cloud Computing Test
Web application built with Spring Boot

## Assignment 5 Test

Created 4 endpoints
        -       GET All uploaded documents of the user
        -       POST  upload a documnet for that user
        -       GET document by ID for that user
        -       DELETE document by ID for that user


## Created a CICD pipeline
-   Created a github action workflow that will run and create AMI on every push request
-   AWS Credentials are set in githib secrets

## Packer file - AMI Creation
-   AMI Creation is done using a packer file 
-   ami.pkr.hcl -> For AMI creation 
-   ami.pkrvars.hcl is a parameter file used as input for ami.pkr.hcl, so change this file for parameterization
-   provision files: 
        1.  setup.sh will create a work a envirnoment on AMI
        2.  java snapshot that will be created during build 
        3.  startup.sh file, that will be triggered on every instance boot-up/reboot

## Build Instructions
-  Clone this repository  into the local system
-  Open the CLI
-  mvn clean install
-  java -jar jar file

## Run the test
-  mvn test

## Kill the process on a port
-  kill $(lsof -t -i:8080)

## Assignment 2
- Create 3 API's, Authenticated GET information by ID, PUT - update information by ID
- Create Public GET

## Testing Workflow

## Assignment 1
-   Created a organization called 'meghanshucloud' and made a repo called webapp
-   Forked the webapp from organization into my personal workspace
-   Created a branch called 'Assignment_!' and pushed my Java SpringBoot application
-   Created an endpoint called healthz on port 3000
-   Endpoint - 'http://localhost:3000/healthz'

--------------------------------------------------------



----------------------------
| Name | NEU ID | Email Address              |
|------| --- |----------------------------|
| Meghanshu Bhatt | 002961585 | bhatt.me@northeastern.edu |

