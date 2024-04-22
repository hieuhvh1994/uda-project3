# Coworking Space Service Extension

The Coworking Space Service is a set of APIs that enables users to request one-time tokens and administrators to authorize access to a coworking space. This service follows a microservice pattern and the APIs are split into distinct services that can be deployed and managed independently of one another.

For this project, you are a DevOps engineer who will be collaborating with a team that is building an API for business analysts. The API provides business analysts basic analytics data on user activity in the service. The application they provide you functions as expected locally and you are expected to help build a pipeline to deploy it in Kubernetes.

## _**Getting Started**_

### Dependencies

##### _Local Environment_

Python Environment - run Python 3.6+ applications and install Python dependencies via pip

Docker CLI - build and run Docker images locally

kubectl - run commands against a Kubernetes cluster

helm - apply Helm Charts to a Kubernetes cluster

--

##### _Remote Resources_

AWS CodeBuild - build Docker images remotely

AWS ECR - host Docker images

Kubernetes Environment with AWS EKS - run applications in k8s

AWS CloudWatch - monitor activity and logs in EKS

GitHub - pull and clone code

## _**SETUP**_

1. Configure AWS account by using `aws configure` cmd.
2. Create Amazon ECR Repository.
3. 

