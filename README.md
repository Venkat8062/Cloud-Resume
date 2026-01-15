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

## Technologies Used
- AWS (S3, CloudFront, IAM)
- GitHub Actions
- HTML / CSS
- Git & GitHub

## Deployment Flow
1. Code changes are pushed to GitHub
2. GitHub Actions pipeline triggers automatically
3. Static files are deployed to S3
4. CloudFront cache is invalidated

## Lessons Learned
- Automating deployments with CI/CD
- Managing static content delivery using CloudFront
- Debugging deployment and permission issues

## Future Improvements
- Infrastructure as Code (Terraform)
- Backend visitor counter using AWS Lambda
- Monitoring and logging
