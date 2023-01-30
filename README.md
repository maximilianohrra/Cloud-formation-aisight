
## CLOUDFORMATION TEMPLATE that creates several interacting microservices // docker container; AWS Lambda //
This YAML template creates an AWS infrastructure that includes an EC2 instance, EC2 security group, public subnet, VPC, Lambda function, IAM role, Docker container, and ECS cluster. The EC2 instance and Lambda function have their configurations specified, while the Docker container and ECS cluster have certain properties set. The template also includes two parameters, ContainerName and ImageName, that can be customized.

# Commands:
# Run infra
Install the AWS CLI on your computer.
Configure the CLI with your AWS credentials using the "aws configure" command.
Create a Cloud Formation template file in YAML or JSON format.
- " aws cloudformation create-stack --stack-name  stack-name --template-body file://path/to/my/template.yaml "

# Verify
> aws cloudformation describe-stacks --stack-name  stack-name

# Update
> aws cloudformation update-stack --stack-name  stack-name --template-body file://path/to/my/template.yaml

# Delete
> aws cloudformation delete-stack --stack-name  stack-name
