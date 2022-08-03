# general-purpose-msoa-platform
A general purpose multi provider service oriented architecture platform so you can build services in convention over configuration design paradigm 

# Pre requirements
All infrastructure is created with terraform and the terraform state is always stored in an S3 bucket regardeless of the cloud provider chosen to deploy the msoa platform to. Therefore in order to start this project you need to:
  - Create an AWS account to hold terraform state
  - Copy the access keys of your root user and add them to your .aws/credentials file.

# Conventions
- Every microservice defines its own infrastructure
- Every microservice should aim for zero dependencies
- A dependency is defined as a shared resource not owned (created) by some particular service
- Infrastructure as code files are alway located at iac directory
- When dependencies are needed they are created in iac/common-infra directory
