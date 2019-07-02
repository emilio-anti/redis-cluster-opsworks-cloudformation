opsworks-redis-cluster-cloudformation
===============================
This is a CloudFormation template that creates an Opsworks Stack to deploy a Redis Cluster. This creates a master layer consisting of 1 master instance and a slave layer consisting of 2 instances.

This template references a github repository containing a Chef cookbook that configures redis-server and the redis-sentinel.

Requirements
------------
You will need an AWS account to deploy this template using CloudFormation.

How it Works
-----
After the template has been used to create the stack in AWS, you can SSH into the master instance and verify the information using the redis-cli. You can pull all of the information to SSH in the EC2 of your account. For this to work you must change or create a new KeyPair and change it in the CloudFormation template.
