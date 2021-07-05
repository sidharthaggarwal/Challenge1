# Challenge1

- Prerequisites
1. We need aws account user with permission to create ALB, EC2 instances , Security group , VPC , Subnets, RDS , Route table  & to run cloud Formation Templates
2. Amazon EC2 SSH key Pair
      Option 1 - You can create key manually using GUI or Using CLI - https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html#having-ec2-create-your-key-pair
      Option 2 - Create key manually on local machine with third party tool and import same  into key pairs on AWS under Network & Security


How to Deploy :

Option 1. Create Stack in Cloud formation on which AWS account you want to create Stack.
Option 2.  Configure aws cli on your machine and using sceret key & Access key to deploy cloud formation template using below command
aws cloudformation deploy --template-file /path_to_template/task.yml --stack-name task-3tier --parameter-overrides DBPass="Value1" KeyName=Value2 --tags Key1=Value1 SSHLocation=Value2


