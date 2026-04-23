# AWS Event Announcement System

A fully serverless event announcement web app built on AWS.
Users can subscribe to events via email and get notified instantly when new events are created.

## Live Architecture
## AWS Services Used

| Service | Purpose |
|---|---|
| Amazon S3 | Hosts the static website frontend |
| Amazon SNS | Sends email notifications to subscribers |
| AWS Lambda | Backend logic for subscribe and create-event |
| API Gateway | Public HTTP endpoints for the frontend |
| AWS IAM | Permissions and security between services |

## Features

- Subscribe to events with your email
- Create new events from the website
- All subscribers get an instant email notification
- Fully serverless — no server to manage
- Free Tier eligible

## How It Works

1. User enters email on the website and clicks Subscribe
2. Lambda function calls SNS to subscribe that email
3. User confirms subscription via email
4. When a new event is created, Lambda publishes to SNS
5. SNS instantly emails all confirmed subscribers

## Tech Stack

- Frontend: HTML, CSS, JavaScript
- Backend: Python 3.12 (AWS Lambda)
- Cloud: AWS (SNS, Lambda, API Gateway, S3, IAM)

## Project Structure
## Author

Built by vishnu0911 as part of an AWS serverless portfolio project.
