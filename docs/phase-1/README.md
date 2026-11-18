# Phase 1: Environment Setup and Workflow Fundamentals

## Project
WanderWise Tours – AI WhatsApp Sales Agent

## 1. Overview
Phase 1 established the technical foundation for developing an AI-powered WhatsApp Sales Agent for WanderWise Tours.

The objective was to prepare the development environment and practise essential n8n workflow concepts.

## 2. Technology Stack
- n8n – Workflow automation and orchestration
- Docker – Containerisation
- PostgreSQL 17 – Database infrastructure
- Git and GitHub – Version control
- JavaScript – Data transformation
- Cursor – Development environment

## 3. Infrastructure Setup
- Configured the local Docker environment.
- Set up and verified the n8n instance.
- Configured PostgreSQL.
- Created a dedicated WanderWise database and database user.
- Configured PostgreSQL credentials in n8n.
- Connected n8n and PostgreSQL through a shared Docker network.

## 4. Workflow Implementation

**Workflow:** WanderWise - Phase 1 - Workflow Fundamentals

| Node | Purpose |
|---|---|
| Manual Trigger | Starts workflow execution |
| Edit Fields | Creates sample customer information |
| Code | Cleans and transforms customer data using JavaScript |
| IF | Checks whether a phone number was provided |

### Data Transformation
The Code node:
- Trims unnecessary whitespace.
- Checks whether a phone number is present.
- Converts the customer name to uppercase.
- Generates a processing timestamp.

### Conditional Routing
The IF node evaluates the `phone_provided` Boolean field:
- **True:** A phone number is available.
- **False:** A phone number is missing.

## 5. Testing
Two scenarios were successfully tested:
1. A customer record containing a phone number.
2. A customer record without a phone number.

Both scenarios produced the expected conditional routing results.

## 6. Outcome
Established the local development environment and implemented a working n8n workflow demonstrating data preparation, JavaScript transformation and conditional routing.

## 7. Next Phase
**Phase 2: WhatsApp Communication**

The next stage will focus on WhatsApp communication in accordance with the internship project plan.

## Project Status
**Phase 1 – Completed**
