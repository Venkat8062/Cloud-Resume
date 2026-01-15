# Cloud Resume Challenge

## Overview
This project implements a cloud-hosted resume website using AWS services.
The goal is to demonstrate hands-on understanding of cloud infrastructure,
deployment, and basic DevOps practices.

## Architecture
- Static website hosted on Amazon S3
- Content delivered globally using CloudFront
- Backend visitor counter implemented with AWS Lambda
- Visitor count stored in Amazon DynamoDB
- CI/CD pipeline using GitHub Actions

## Backend Visitor Counter
A serverless backend is implemented to track page visits.

- AWS Lambda handles HTTP requests from the frontend
- Amazon DynamoDB stores and updates the visitor count
- API is invoked from the frontend using JavaScript
- IAM policies follow least-privilege principles

## Technologies Used
- AWS (S3, CloudFront, IAM)
- GitHub Actions
- HTML / CSS
- Git & GitHub

## Deployment Flow
1. Frontend code is pushed to GitHub
2. GitHub Actions pipeline deploys static files to S3
3. CloudFront cache is invalidated automatically
4. Lambda function processes visitor count requests
5. DynamoDB persists visitor data

## Lessons Learned
- Automating deployments with CI/CD
- Managing static content delivery using CloudFront
- Debugging deployment and permission issues

## Future Improvements
- Infrastructure as Code (Terraform)
- Backend visitor counter using AWS Lambda
- Monitoring and logging

## Observability (Design Consideration)
AWS CloudWatch can be used to monitor Lambda execution,
track errors, and debug request flows. In a production
setup, logs and metrics would be actively monitored
to ensure reliability.
