# Postman API Automation with Github Actions #

This repository is a demonstration for POC for integrating postman tests with github actions. The Tests are written in Postman and they are executed on the VM with the help of newman and newman-reporter-htmlextra.
Github Actions will trigger the project execution on every push to the main branch. You can also execute the project manually using workflow_dispatch. The Projects runs on a scheduled time with the help of the cron job.

The HTML report is archieved and kept in the artifact section for the team to download it. Along with that they can view the report directly from the github page.
