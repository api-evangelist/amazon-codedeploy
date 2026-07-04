---
title: "Blue/Green Deployments to Amazon ECS using AWS CloudFormation and AWS CodeDeploy"
url: "https://aws.amazon.com/blogs/devops/blue-green-deployments-to-amazon-ecs-using-aws-cloudformation-and-aws-codedeploy/"
date: "2024-06-19"
author: "Ajay Mehta"
feed_url: "https://aws.amazon.com/blogs/devops/tag/aws-codedeploy/feed/"
---
Introduction Many customers use Amazon Elastic Container Service (ECS) for running their mission critical container-based applications on AWS. These customers are looking for safe deployment of application and infrastructure changes with minimal downtime, leveraging AWS CodeDeploy and AWS CloudFormation . AWS CloudFormation natively supports performing Blue/Green deployments on ECS using a CodeDeploy Blue/Green hook , but this feature comes with some additional considerations that are outlined here ; one of them is the inability to use CloudFormation nested stacks, and another is the inability to update application and infrastructure changes in a single deployment.
