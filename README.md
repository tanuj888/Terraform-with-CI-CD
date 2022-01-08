![This is an image](https://github.com/tanuj888/Terraform-with-CI-CD/blob/main/Terraform.png)

## Project Title -Terraform-with-CI-CD
This project is used to deploy Infrastructurelike VPC,subnets through terraform and automating it with the help of Jenkins CI/CD pipeline.
## Project Description
This Project contains a full, real-world solution for setting up an environment using DevOps technologies and practices for deploying cloud services/cloud infrastructure like Virtual Private Cloud to AWS.
## Technology Used/Details
You will be using the following technologies and platforms to set up a DevOps environment.
1. AWS 
   - AWS will be used to host the application, cloud infrastructure, and any other services we may need to ensure the VPC is deployed properly.
2. GitHub
   - To store the application and infrastructure/automation code
3. Terraform
   - To automate the infrastructure deployment on AWS 
4. Jenkins CI/CD
    - Used Jenkins  to create CI and CD pipeline
5. Git bash
    - This tool is ues to SSH in EC2 instance and to push local files to git hub

## Prerequisites
1. **AWS EC2** linux/ubuntu instance
2. Configure **Jenkins** on the AWS instance by following the steps mentioned [here](https://www.jenkins.io/doc/tutorials/tutorial-for-installing-jenkins-on-AWS/)
3. Install necessay plugin on Jenkins like **Terraform, Github**.
4. **Install Terraform** on the same EC2 instance by following the steps mentioned [here](https://learn.hashicorp.com/tutorials/terraform/install-cli)
5. **Install git** on the instance by `sudo yum install git -y`
6. Integrate/Configure **Github with Jenkins** by following the steps [here](https://www.blazemeter.com/blog/how-to-integrate-your-github-repository-to-your-jenkins-project)
7. Create an **IAM role** with full **administrative access** and attach it to the EC2 instance.

## Steps Performed in the Project
1. Created a directory in local machine and crated two terraform files-
     - Provider.tf to mention the AWS provided with the region defined. [Reference](https://registry.terraform.io/providers/hashicorp/aws/latest/docs)
     - VPC.tf to mentioned the virtual private cloud components. [Reference](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/vpc)
     
2. ## Push the code in Github
 ````
 git init -x main
 git add .
 git commit -x "initial commit"
 git remote add origin  <REMOTE_URL> 
 git remote -v
 git push origin main/master
 
 ````
 
