# demo

A demo Django Application that uses AWS RDS as Backend Database 

Framework - Django v4.2.7  ; Backend DB - AWS RDS



## Setup and Workflow

The git repository contains a Django Project. A Dockerfile has been created to Dockerize the given Project.

The repository is also configured with TWO Different Github Actions Workflows :

1. **Build and Push Docker Image to ECR** - This workflow builds the docker Image of the given Django Project application. After the build process is completed, it authenticates to the AWS ECR Repository and the docker Image is pushed to the remote ECR Repository.

2. **Semgrep** - This workflow runs on each Pull Request as well as any merge to master/main branch of the project. Semgrep has been configured to run with Django specific ruleset to identify vulnerabilities related to Django framework.

   



