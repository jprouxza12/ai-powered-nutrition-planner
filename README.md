# AI-Powered Nutrition Plan Generator

## Description
An intelligent web application that generates personalized nutrition and meal plans using AWS services and AI. The application calculates individual caloric needs using various scientific formulas, considers activity levels, fitness goals, and dietary restrictions to create comprehensive, customized nutrition plans.

## Features
- Multiple BMR calculation methods:
  - Mifflin-St Jeor Formula
  - Harris-Benedict Formula
  - Katch-McArdle Formula
  - WHO Formula
- Customizable activity level multipliers
- Various fitness goal options:
  - Fat loss (slow/moderate/aggressive)
  - Maintenance
  - Muscle gain (slow/moderate/aggressive)
- Food allergy considerations
- Detailed macronutrient distribution
- 7-day meal plan generation
- Shopping list organization
- Meal prep instructions
- PDF download functionality

## Technology Stack
- Frontend:
  - HTML5
  - CSS3
  - JavaScript
- Backend:
  - Python
  - AWS Lambda
  - Amazon Bedrock (Claude 3 Sonnet)
  - Amazon S3
  - AWS SDK
- Authentication:
  - Amazon Cognito

## Architecture
```mermaid
graph LR
    A[Web Interface] --> B[API Gateway]
    B --> C[Lambda Function]
    C --> D[Amazon Bedrock]
    C --> E[Amazon S3]
    C --> F[Cognito]
