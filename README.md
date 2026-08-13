# ORLIX AI Customer Service SaaS

A production-deployed, multi-company AI customer service platform designed to help businesses automate customer conversations, manage support teams, train AI assistants, and provide real-time support through website chat and messaging channels.

> This is the public portfolio repository. Production source code, credentials, customer data, internal administration tools, and deployment configuration remain private.

## Product Overview

ORLIX AI Customer Service SaaS combines artificial intelligence, customer support workflows, multi-tenant infrastructure, live chat, knowledge management, and operational dashboards in one platform.

The platform is built as a real SaaS product rather than a standalone chatbot. Each company can operate in an isolated workspace with its own customers, conversations, AI configuration, knowledge base, and support workflow.

## Current Capabilities

- AI-powered automatic customer replies
- OpenAI and Google Gemini provider support
- Professional unified customer service inbox
- Human agent handover
- AI Training Center with company-specific configuration
- Knowledge Base and document ingestion
- PDF and DOCX parsing
- Embeddable website live chat widget
- Multi-company / multi-tenant workspace isolation
- Customer and conversation management
- Agent assignment, notes, tags, priority, and conversation status
- Client dashboard
- Secure Owner / Platform administration
- Trial and product-management foundation
- Analytics foundation
- Telegram integration foundation
- Multi-industry and multilingual customer support

## Production & Quality Validation

The private production repository includes automated validation for application startup, database migrations, required routes, Python and JavaScript syntax, authentication boundaries, and runtime security checks.

The platform is deployed under the ORLIX domain and uses a production smoke-test workflow to validate the live service after deployment.

## Technology Stack

- FastAPI
- Python
- SQLAlchemy
- PostgreSQL
- Alembic
- Redis
- WebSocket
- OpenAI
- Google Gemini
- Docker
- GitHub Actions

## Architecture

```text
Customer
   |
   v
Website Live Chat / Messaging Channels
   |
   v
ORLIX API Gateway & Customer Service Backend
   |
   +--> Authentication & Tenant Isolation
   +--> Conversation Engine
   +--> AI Training & Knowledge Base
   +--> AI Provider Layer (OpenAI / Gemini)
   +--> Human Agent Inbox
   +--> Analytics & Platform Administration
   |
   v
PostgreSQL + Redis
```

## Portfolio Documentation

- [Product Features](FEATURES.md)
- [Architecture](ARCHITECTURE.md)
- [Security](SECURITY.md)
- [Product Roadmap](ROADMAP.md)
- [Demo Information](DEMO.md)

## Public / Private Boundary

This repository intentionally contains portfolio documentation only. The following remain private:

- Production application source code
- API keys and environment variables
- Customer and conversation data
- Production database credentials
- Internal ORLIX administration code
- Deployment secrets and infrastructure configuration
- Internal AI prompts and security controls

## Project Status

**Active product development and production validation.**

The core AI Customer Service SaaS foundation is implemented and deployed. Current work focuses on production hardening, broader omnichannel integrations, billing, monitoring, and continued product improvement.

## ORLIX

ORLIX builds AI systems designed to work alongside humans in real operational environments.

Product: **ORLIX AI Customer Service SaaS**  
Website: `orlix.tech`
