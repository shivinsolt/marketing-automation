# MannKaa QR Marketing Platform

A serverless QR code marketing and analytics platform built with AWS Lambda, DynamoDB, API Gateway (CloudFormation), and Appsmith.

## Architecture
- **AWS Region**: us-east-2
- **Infrastructure**: AWS CloudFormation (`template.yaml`)
- **Database**: DynamoDB (`QRCampaigns`, `QRScans`)
- **Compute**: Node.js 20.x AWS Lambda (`QRRedirectEngine`)
- **Frontend**: Appsmith Dashboard

## Deployment Steps
1. Log in to the AWS Management Console and navigate to **CloudFormation**.
2. Create a new stack by uploading the `template.yaml` file.
3. Set the region to `us-east-2`.
4. Once deployment is complete, copy the `BaseApiUrl` from the stack Outputs tab.
5. Import the API endpoints into your Appsmith dashboard to manage campaigns and view real-time scan analytics.