# Minimnal serverless api DynamoDB

A barebones serverless [Express](https://expressjs.com/) API template using Pulumi's cloud.HttpServer built on AWS API Gateway and Lambda functions, serving a dynamic DynamoDB-based hit counter.

- Pulumi
- AWS Lambda
- AWS API Gateway
- AWS DynamoDB

## run

```bash
# Deploy resources:
pulumi up

# Test the endpoint:
pulumi stack select
for i in {1..5}; do curl $(pulumi stack output url); done

# Clean up resources:
pulumi destroy
pulumi stack rm
```

## todo

- Linting with Prettier
- Testing with jest
- Gitpod support

Based on: [awsworkshop.com](https://pulumi.awsworkshop.io/additional-content/120_serverless_application_patterns/1_new_project.html)
