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
- API documentation via Swagger for clear endpoint reference.

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
