# hono-aws

This repository contains a sample codebase for setting up a serverless function using Hono with AWS Lambda, orchestrated by AWS CDK for easy deployment.

## Introduction

The `hono-aws` project demonstrates how to deploy a Hono.js application as an AWS Lambda function, with the AWS Cloud Development Kit (CDK) managing the infrastructure. This approach offers a scalable, cost-effective, and easy-to-manage serverless backend solution.

## Prerequisites

Before you begin, ensure you have the following installed:

- Node.js (version 14.x or later)
- AWS CLI (configured with your AWS account)
- AWS CDK Toolkit

## Installation

To set up the `hono-aws` stack, follow these steps

```
git clone https://github.com/rokasta12/hono-aws.git
cd hono-aws
npm install
npm run build
npx cdk deploy
```

Upon successful deployment, the AWS CDK will provide you with the endpoint URL of the deployed Hono Lambda function.

## Usage

Once the stack is deployed, you can interact with the Hono Lambda function through the following HTTP requests:


```
curl https://<your-lambda-url>/read
```

*Note: Be sure to replace `<your-lambda-url>` with the actual URL provided post-deployment.*


## Support and Contributions

If you run into any problems or have suggestions, please open an issue in the repository. Contributions to enhance `hono-aws` are welcomed. Feel free to fork the repository and submit a pull request with your improvements.

## License

The `hono-aws` project is open-sourced under the MIT license.
