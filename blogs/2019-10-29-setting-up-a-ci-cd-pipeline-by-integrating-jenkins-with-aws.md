---
title: "Setting up a CI/CD pipeline by integrating Jenkins with AWS CodeBuild and AWS CodeDeploy"
url: "https://aws.amazon.com/blogs/devops/setting-up-a-ci-cd-pipeline-by-integrating-jenkins-with-aws-codebuild-and-aws-codedeploy/"
date: "2019-10-29"
author: "Noha Ghazal"
feed_url: "https://aws.amazon.com/blogs/devops/tag/aws-codedeploy/feed/"
---
In this post, I explain how to use the Jenkins open-source automation server to deploy AWS CodeBuild artifacts with AWS CodeDeploy , creating a functioning CI/CD pipeline. When properly implemented, the CI/CD pipeline is triggered by code changes pushed to your GitHub repo, automatically fed into CodeBuild, then the output is deployed on CodeDeploy. Solution overview The functioning pipeline creates a fully managed build service that compiles your source code.
