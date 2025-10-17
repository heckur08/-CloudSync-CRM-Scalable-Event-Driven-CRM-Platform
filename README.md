# CloudSync CRM: Scalable Event-Driven CRM Platform

## Overview
CloudSync CRM is a distributed microservices platform designed to manage orders, customers, and inventory efficiently. It leverages event-driven architecture with AWS SQS for asynchronous messaging and AWS Lambda for serverless processing. The system uses a hybrid data model with PostgreSQL for relational data and DynamoDB for flexible non-relational storage, while ElasticSearch and Redis optimize search and caching operations.

---

## Features
- Built with TypeScript and NestJS for a modular and maintainable backend.
- Utilizes AWS SQS for reliable, scalable message queuing and asynchronous processing.
- Serverless AWS Lambda functions execute background jobs and event-driven workflows.
- Hybrid database usage: PostgreSQL for transactional consistency, DynamoDB for flexible storage.
- ElasticSearch integration provides advanced search and analytics capabilities.
- Redis caching enhances performance for frequent queries and queue management.
- Containerized with Docker for consistent deployment in diverse environments.
- API documentation via Swagger for a clear endpoint reference.

---

## Technologies Used
- TypeScript, Node.js
- NestJS framework
- AWS SQS & Lambda services
- PostgreSQL & DynamoDB databases
- ElasticSearch & Redis
- Docker containerization
- Swagger for API documentation

---

## Installation & Setup

### Prerequisites
Ensure you have installed and configured:
- Node.js (v16+)
- Docker
- AWS account with proper permissions for SQS, Lambda, DynamoDB, and RDS
- PostgreSQL instance credentials

### Clone the Repository and Install Dependencies
```
git clone https://github.com/yourusername/cloudsync-crm.git
cd cloudsync-crm
npm install
```
### Configure Environment Variables
Create a `.env` file in the root directory and provide the following (sample):
```
AWS_ACCESS_KEY_ID=your_access_key
AWS_SECRET_ACCESS_KEY=your_secret_key
DATABASE_HOST=your_db_host
DATABASE_PORT=5432
DATABASE_USERNAME=your_db_user
DATABASE_PASSWORD=your_db_password
SQS_QUEUE_URL=your_sqs_queue_url
DYNAMODB_REGION=your_aws_region
ELASTICSEARCH_HOST=your_elasticsearch_endpoint
REDIS_HOST=your_redis_host
```
### Running Locally
- Without Docker:
```
npm run start:dev
```
- Using Docker:
```
docker build -t cloudsync-crm .
docker run -p 3000:3000 cloudsync-crm
```
---

## Architecture Overview
CloudSync CRM is composed of multiple microservices communicating asynchronously via AWS SQS queues and Lambda functions. The API Gateway handles HTTP requests and routes them appropriately. Data persistence spans relational and NoSQL databases, optimized search is facilitated by ElasticSearch, while Redis improves cache and queue performance. Docker ensures environment consistency from development to production.

---

## Future Enhancements
- Implement full-fledged service discovery and circuit breakers for resilience.
- Extend API with real-time WebSocket notifications.
- Automate deployment using Terraform or CloudFormation.
- Add comprehensive monitoring and logging with AWS CloudWatch and ELK stack.

---

## Contribution
Contributions are encouraged. Please submit issues or pull requests for suggestions and fixes.

---

## License
This project is MIT licensed.
