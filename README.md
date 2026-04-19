# Amazon CodeDeploy

AWS CodeDeploy is a fully managed deployment service that automates software deployments to various compute services such as Amazon EC2, AWS Fargate, AWS Lambda, and on-premises servers. CodeDeploy makes it easier to rapidly release new features, helps avoid downtime during application deployment, and handles the complexity of updating your applications with in-place, blue/green, and canary deployment strategies.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Amazon, AWS, Deployment, DevOps, CI/CD, Release Management, Blue/Green Deployment

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-04-19

## APIs

### Amazon CodeDeploy API

The Amazon CodeDeploy REST API enables programmatic management of applications, deployment groups, deployment configurations, and deployments. Create and update deployment groups, trigger deployments to EC2, Lambda, ECS, and on-premises targets, monitor deployment status, and manage deployment lifecycle hooks and rollback policies.

**Human URL:** [https://docs.aws.amazon.com/codedeploy/latest/APIReference/Welcome.html](https://docs.aws.amazon.com/codedeploy/latest/APIReference/Welcome.html)

#### Tags:

 - Amazon, AWS, Deployment, DevOps, CI/CD

#### Properties

- [Documentation](https://docs.aws.amazon.com/codedeploy/latest/userguide/welcome.html)
- [APIReference](https://docs.aws.amazon.com/codedeploy/latest/APIReference/Welcome.html)
- [OpenAPI](openapi/amazon-codedeploy-openapi-original.yaml)

## Common Properties

- [GettingStarted](https://docs.aws.amazon.com/codedeploy/latest/userguide/getting-started-codedeploy.html)
- [Authentication](https://docs.aws.amazon.com/codedeploy/latest/userguide/auth-and-access-control.html)
- [Pricing](https://aws.amazon.com/codedeploy/pricing/)
- [Console](https://console.aws.amazon.com/codedeploy/)
- [Portal](https://aws.amazon.com/codedeploy/)
- [Documentation](https://docs.aws.amazon.com/codedeploy/latest/userguide/)
- [TermsOfService](https://aws.amazon.com/service-terms/)
- [PrivacyPolicy](https://aws.amazon.com/privacy/)
- [StatusPage](https://health.aws.amazon.com/health/status)
- [Blog](https://aws.amazon.com/blogs/devops/)
- [FAQ](https://aws.amazon.com/codedeploy/faqs/)
- [SignUp](https://portal.aws.amazon.com/gp/aws/developer/registration/index.html)
- [GitHubOrganization](https://github.com/aws)

## Features

| Name | Description |
|------|-------------|
| Multiple Deployment Strategies | Support for in-place, blue/green, and canary deployment strategies across EC2, Lambda, ECS, and on-premises targets to m |
| Automated Rollbacks | Automatically roll back deployments if a specified number of instances fail health checks or if CloudWatch alarms are tr |
| Deployment Lifecycle Hooks | Define custom lifecycle event hooks (BeforeInstall, AfterInstall, ApplicationStart, etc.) using scripts or Lambda functi |
| Traffic Shifting for Lambda and ECS | Implement canary and linear traffic shifting for Lambda function updates and ECS service deployments with configurable t |
| Deployment Groups | Organize deployment targets using deployment groups with EC2 instance tags, Auto Scaling groups, ECS clusters, or on-pre |
| CodeDeploy Agent | Install the CodeDeploy agent on EC2 or on-premises instances to enable deployment target registration and lifecycle hook |
| Integration with AWS Load Balancers | Integrate with Application Load Balancers and Network Load Balancers for blue/green deployments that shift traffic betwe |

## Use Cases

| Name | Description |
|------|-------------|
| Zero-Downtime Application Updates | Use blue/green deployments to update applications without downtime by routing traffic to a new environment while keeping |
| Lambda Function Updates | Deploy new Lambda function versions with canary or linear traffic shifting to gradually migrate traffic from the current |
| ECS Service Deployment | Deploy updated container tasks to ECS services with blue/green deployments and configurable traffic shifting through an  |
| On-Premises Application Deployment | Extend cloud-based deployment automation to on-premises servers using the CodeDeploy agent and on-premises instance regi |
| Multi-Stage CD Pipeline | Use CodeDeploy as the deployment stage in an AWS CodePipeline for fully automated continuous delivery from source code t |

## Integrations

| Name | Description |
|------|-------------|
| AWS CodePipeline | Use CodeDeploy as the deployment stage in CodePipeline CD pipelines. |
| AWS CodeBuild | Trigger CodeDeploy deployments from build artifacts produced by CodeBuild. |
| AWS Lambda | Deploy Lambda function updates with traffic shifting strategies. |
| Amazon ECS | Deploy ECS service updates with blue/green deployments. |
| AWS CloudWatch | Trigger automatic rollbacks based on CloudWatch alarm states. |
| Elastic Load Balancing | Integrate with ALB and NLB for blue/green traffic shifting. |
| Amazon EC2 Auto Scaling | Deploy to Auto Scaling groups with automatic instance health checking. |
| AWS Systems Manager | Use SSM Run Command and State Manager for deployment automation. |
| GitHub | Deploy application revisions stored in GitHub repositories. |
| Amazon S3 | Store and retrieve application deployment bundles from S3. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [amazon-codedeploy-openapi-original](openapi/amazon-codedeploy-openapi-original.yaml)
- [amazon-codedeploy-openapi](openapi/amazon-codedeploy-openapi.yml)

### JSON Schema

394 JSON Schema files generated from the OpenAPI specification.

- [amazon-codedeploy-add-tags-to-on-premises-instances-input-schema](json-schema/amazon-codedeploy-add-tags-to-on-premises-instances-input-schema.json)
- [amazon-codedeploy-additional-deployment-status-info-schema](json-schema/amazon-codedeploy-additional-deployment-status-info-schema.json)
- [amazon-codedeploy-alarm-configuration-schema](json-schema/amazon-codedeploy-alarm-configuration-schema.json)
- [amazon-codedeploy-alarm-list-schema](json-schema/amazon-codedeploy-alarm-list-schema.json)
- [amazon-codedeploy-alarm-name-schema](json-schema/amazon-codedeploy-alarm-name-schema.json)
- ...and 389 more in [json-schema/](json-schema/)

### JSON Structure

393 JSON Structure files in [json-structure/](json-structure/).

### JSON-LD

- [amazon-codedeploy-context](json-ld/amazon-codedeploy-context.jsonld)

### Examples

393 example JSON files in [examples/](examples/).

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [codedeploy](capabilities/shared/codedeploy.yaml) — 47 operations

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Amazon CodeDeploy Deployment Automation](capabilities/amazon-codedeploy-deployment-automation.yaml) | codedeploy | 10 | DevOps Engineer |

## Vocabulary

- [amazon-codedeploy-vocabulary](vocabulary/amazon-codedeploy-vocabulary.yaml) — Unified taxonomy mapping 1 resources, 6 actions, 1 workflows, and 2 personas

## Rules

- [amazon-codedeploy-spectral-rules](rules/amazon-codedeploy-spectral-rules.yml) — 9 rules enforcing Amazon CodeDeploy API conventions

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
