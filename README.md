# Cloud Computing Final Exam

## Description

This project implements Infrastructure as Code (IaC) in AWS using AWS CloudFormation and GitHub Actions.

The infrastructure includes:

* Security Groups
* EC2 Instance with Elastic IP
* Application Load Balancer
* Target Group
* Launch Template
* Auto Scaling Group
* Warm Pool
* Scheduled Scaling Actions

All deployments are automated through GitHub Actions.

## Repository Structure

```text
cloudformation/
    security.yml
    ec2.yml
    alb-asg.yml
    automation.yml

.github/workflows/
    deploy.yml
    destroy.yml
```

## Deployment

The deployment is executed through:

* deploy.yml

The workflow creates all CloudFormation stacks in the correct order.

## Destruction

The destruction is executed through:

* destroy.yml

The workflow removes all stacks in reverse dependency order.

## Technologies

* AWS CloudFormation
* AWS EC2
* AWS Elastic Load Balancer
* AWS Auto Scaling
* GitHub Actions

## Author

Juan Jose Quin
Julian Andres Vergel
Cloud Computing - Final Exam
