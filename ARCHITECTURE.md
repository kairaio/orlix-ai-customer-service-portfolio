# System Architecture

## High-Level Architecture

```mermaid
flowchart TD
    Customer[Customer] --> Widget[Website Live Chat Widget]
    Customer --> Channel[Messaging Channel]
    Widget --> API[FastAPI Application]
    Channel --> API
    Agent[Support Agent] --> Inbox[Professional Inbox]
    Owner[Company Owner] --> Dashboard[Owner Dashboard]
    Inbox --> API
    Dashboard --> API
    API --> Auth[Authentication and Tenant Layer]
    API --> Conversation[Conversation Services]
    API --> AI[AI Engine]
    API --> KB[Knowledge Base]
    API --> DB[(PostgreSQL)]
    API --> Redis[(Redis)]
    AI --> OpenAI[OpenAI]
    AI --> Gemini[Google Gemini]
    AI --> KB
```

## Backend Layers

```text
API Layer
    ↓
Service Layer
    ↓
Repository Layer
    ↓
SQLAlchemy Models
    ↓
PostgreSQL
```

## Multi-Tenant Design

Tenant isolation is applied to company data, contacts, conversations, messages, AI settings, Knowledge Base content, widget configuration, and team members.
