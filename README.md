# aws-lambda-serverless-api

Simple serverless API using AWS Lambda and API Gateway.

## Architecture

Client → API Gateway → Lambda Function

A client sends an HTTP request to API Gateway.  
API Gateway triggers an AWS Lambda function that returns a JSON response.

## Technologies Used

- AWS Lambda
- Amazon API Gateway
- Python
- Serverless architecture
- GitHub (version control)

## Setup Steps

1. Create an AWS account.
2. Go to the AWS Console.
3. Navigate to AWS Lambda.
4. Click "Create Function".
5. Choose "Author from scratch".
6. Select Python runtime.
7. Upload or paste the Lambda function code.
8. Save the function.
9. Test the Lambda function in the AWS console.

## Deployment Steps

1. Go to Amazon API Gateway.
2. Create a new HTTP API.
3. Add your Lambda function as the integration.
4. Create a route (for example GET /hello).
5. Deploy the API.
6. Copy the Invoke URL.

## Sample Event

Example request sent to the API:

{
  "message": "test request"
}

## Example Response

{
  "statusCode": 200,
  "body": "Hello from AWS Lambda!"
}

## Lambda Code Explanation

The Lambda function receives a request from API Gateway and returns a simple message.

When the API endpoint is called, API Gateway triggers the Lambda function.  
The function processes the request and returns a response with status code 200 and a message.

## Project Purpose

This project was created to practice serverless architecture on AWS using Lambda and API Gateway.

It demonstrates how to build and deploy a simple API without managing servers.
