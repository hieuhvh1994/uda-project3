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
2. Create Amazon ECR Repository: Create ECR Repository to store your image
3. Create Amazon CodeBuild: Use CodeBuild to connect to your GitHub Repository to trigger your build.
4. Create buildspec.yaml: This file would contain who you can build and push Docker image to ECR.
5. Push Changes to GitHub: Make changes and push to you repository.
6. CodeBuild: The CodeBuild will automatically trigger your changes to build image and push to ECR.
7. Enter cmd `kubectl apply -f configmap.yaml` to apply config properties and secret.
8. Enter cmd `kubectl apply -f coworking.yaml` to deploy coworking app.

## _Stand-Out Suggestions_

1. ##### Reasonable Memory and CPU Allocation
We should specify reasonable Memory and CPU Allocation to ensure optimal the application performance.

2. ##### Best AWS Instance Type
The best AWS Instance Type would be depended on the factors such as workload or traffic. Based on the requirement, we should choose the suitable instant type for the application.

3. ##### Cost Optimization Strategies
To reduce the costs, we should implement auto-scaling to dynamically adjust resources based on demand, leverage instances and containers for resource usage and use cost management tools to monitor the costs.