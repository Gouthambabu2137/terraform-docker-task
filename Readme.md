# Task 3: Infrastructure as Code (IaC) with Terraform

## Project Overview

This project demonstrates the use of Terraform to provision and manage infrastructure in the form of a local Docker container. The goal of this task was to implement Infrastructure as Code (IaC) principles by automating the deployment and teardown of a Docker-based Nginx web server.

## Tools and Technologies Used

- Terraform
- Docker
- Git and GitHub

## Objective

- Automate container provisioning using Terraform.
- Understand and apply key Terraform commands.
- Manage Docker infrastructure through code.

## Task Execution Summary

1. Created a project directory named `terraform-docker-task`.

2. Created a `main.tf` configuration file with:
   - Docker provider (`kreuzwerker/docker`)
   - A Docker image resource (`nginx:latest`)
   - A Docker container resource (`my-nginx-container`) mapped to host port `8080`

3. Initialized Terraform using:
   terraform init

4. Validated configuration using:
   terraform plan

5. Applied the configuration and provisioned the container using:
   terraform apply

6. Verified that the Nginx container was running by visiting:
   http://localhost:8080

7. Inspected Terraform-managed resources using:
   terraform state list

8. Cleaned up the infrastructure using:
   terraform destroy


9. Captured the full output of all Terraform operations in `execution_log.txt`.

10. Pushed the project to a GitHub repository for submission.

## Files Included

- `main.tf` – Terraform configuration file
- `execution_log.txt` – Log of all Terraform command executions
- `.gitignore` – To exclude system and Terraform-generated files
- `terraform.tfstate` and related files (auto-generated)

## Repository Link

[https://github.com/Gouthambabu2137/terraform-docker-task](https://github.com/Gouthambabu2137/terraform-docker-task)

## Author

Goutham Babu  
Intern, Kodestree Technology  
GitHub: [@Gouthambabu2137](https://github.com/Gouthambabu2137)
