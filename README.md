# Automated-analysis-on-AWS
The Automated Data Analytics on AWS solution provides an end-to-end data platform for ingesting, transforming, managing and querying datasets. This helps analysts and business users manage and gain insights from data without deep technical experience using Amazon Web Services (AWS). It has an open-sourced architecture with connectors to commonly used AWS services, along with third-party data sources and services. This solution also provides an user interface (UI) to search, share, manage, and query datasets using standard SQL commands.

# Architecture overview
<img width="1376" height="792" alt="solution_architecture_diagram" src="https://github.com/user-attachments/assets/bd60766a-1d67-4e62-99b7-b4286b773921" />
The Automated Data Analytics on AWS solution automates the building of data pipelines that are optimized for the size, frequency of update, and type of data. These data pipelines handle the data ingestion, transformations, and queries.

The Automated Data Analytics on AWS solution creates and integrates a combination of AWS services required to perform these tasks, abstracted through a user interface. These services include AWS Glue crawlers, jobs, workflows and triggers, along with S3 buckets, IAM integration, and other services. Additionally, the solution automatically detects and redacts personally identifiable information (PII) with granular security and governance controls.

# Prerequisites
# Build environment specifications
To build and deploy this solution, we recommend using Ubuntu with minimum 4 cores CPU, 16GB RAM. Mac(Intel) or other Linux distributions are also supported.
The computer used to build the solution must be able to access the internet
# AWS Account
A CDK bootstrapped AWS account.
(https://docs.aws.amazon.com/cdk/latest/guide/bootstrapping.html)
# Sufficient AWS Lambda Concurrent executions limit

Please use AWS Service Quotas to verify AWS Lambda Concurrent executions Applied quota value in your account is greater or equal to the AWS default quota value (which is 1000). Click this link to check it in your AWS Console. If Applied quota value is less than 1000, please use Request quota increase button to make a request to increase it to at least 1000 before deploying the solution. 
# Tools
* The latest version of the AWS CLI, installed and configured.
* (https://aws.amazon.com/cli/ .)

node.js version 18.19.

(https://docs.npmjs.com/getting-started)
Below are the example commands for installing nvm and node 18, please make sure those commands fit your build environment before using them.
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.2/install.sh | bash
exec $SHELL -l
nvm install 18.19


