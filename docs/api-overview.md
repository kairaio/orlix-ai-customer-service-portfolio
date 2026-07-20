# API Overview

The production API is built with FastAPI.

Major API groups include authentication, companies, contacts, conversations, messages, Professional Inbox, AI Training, Knowledge Base, live chat, widget, trial, dashboard, and integrations.

Example health response:

```json
{
  "status": "healthy",
  "service": "AI Customer Service SaaS"
}
```

Protected endpoints use bearer-token authentication.
