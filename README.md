## Postman API Automation Integration with Github Actions ##
This repository is a demonstartion for POC for integrating postman with github actions. The tests are written in Postman and they are executed on the VM with the help of newman and newman-reporter-htmlextra. Github Actions will trigger the project execution on every push to the main branch. You can also execute the project manually using workflow_dispatch. The Projects run on a scheduled time with the help of the cron job.

The HTML reports is archieved and kept in the artifact section for the team to download it. Along with that they can view the report directly from the github page. The latest report is mailed to the team members using GMAIL SMTP.

## About Me ##
Hi My name is Mukesh Upadhyay. I have 3+ years of experience into Manual and  Automation Testing. My skillset includes UI Automation with Selenium Webdriver, Playwright and for API Testing I use Rest Assured and Postman. You can connect with me over: (https://www.linkedin.com/in/mukesh-u-226205127/)

## Testing Coverage ##

1. Happy Flow Testing
2. Negative Testing and Edge Case Testing
3. Token Testing
4. Schema Validation
5. Secrets Management with Github Secrets

## Tech Stack ##

1. Postman
2. Nodejs 22v
3. Newman
4. Newman-Reporter-Htmlextra
5. Github Actions

## HTML Report ##
The report will be created in the newman folder Postman Report

## Project Structure ##
```
Phoenix-Inwarranty-Flow
├─ Inwarranty-flow Collection.postman_collection.json # Collection File
├─ QA.postman_environment.json # Environment File
```


## How to run the Project? ##
You can run the project on your local system for that:

1. Clone the Project on Local System: https://github.com/mukesh-u/Postman-In-warranty-flow-API-Collection.git
2. Install Nodejs and NPM from https://nodejs.org/en
3. Install Newman using ```npm install -g newman```
4. Instal Newman-reporter-htmlextra ```npm install -g newman-reporter-htmlextra```
5. Run the Newman Command:
```
              newman run 'Inwarranty-flow Collection.postman_collection.json' \  
             -e QA.postman_environment.json \
             -d testData.csv \
             -r cli,htmlextra \
             --reporter-htmlextra-export ./newman/index.html
```
