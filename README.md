# Particle41 DevOps Challenge

## Project Overview
This project contains a minimal web service `SimpleTimeService`, a Dockerized Python application, and Terraform code for deploying the service on AWS using ECS.

## Steps to Deploy

### 1. Build and Run the Docker Container
To build and run the container, execute the following:

```bash
docker build -t amitjagtap/simpletimeservice:latest .
docker run -p 8080:8080 amitjagtap/simpletimeservice:latest
```

### 2. Terraform Infrastructure Deployment
To deploy the infrastructure using Terraform, run the following:

```bash
terraform init
terraform plan
terraform apply
```

This will provision the necessary infrastructure, including ECS service and an ALB.
