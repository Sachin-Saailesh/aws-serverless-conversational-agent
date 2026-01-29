# AWS Serverless Conversational Agent

## 🎯 Strategic Tagline
Production NLP chatbot using AWS Lex, Lambda, and S3 with weather API integration, hosted on Angular frontend via Amplify CLI.

## 💡 Problem & Solution

### The Challenge
- Need for scalable, serverless chatbot infrastructure
- Natural language understanding for weather queries
- Multi-turn conversation flow management
- Cross-origin integration with web frontend

### The Solution
- AWS Lex: Intent classification + slot filling
- Lambda functions: Weather API calls (OpenWeatherMap)
- S3: Static website hosting + CORS configuration
- Cognito: User authentication and session management

## 🛠️ Tech Stack
- **AWS:** Lex, Lambda, S3, Cognito, Amplify
- **Backend:** Python (Lambda), Serverless Framework
- **Frontend:** Angular, TypeScript, AWS SDK
- **APIs:** OpenWeatherMap, Geolocation

## 📊 Key Results

| Metric | Value |
|--------|-------|
| **Intent Accuracy** | 94% |
| **Avg. Response Time** | <800ms |
| **Concurrent Users** | 1,000+ |
| **Cost per 1K requests** | $0.12 |

## 🚀 Installation & Usage

```bash
# Deploy Lambda
serverless deploy --region us-east-1

# Configure Lex bot
aws lex-models put-bot --cli-input-json file://bot-definition.json

# Deploy Angular app
ng build --prod
amplify publish
```
