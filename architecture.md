# Architecture

## Overview

The system is designed as a lightweight cloud-based application for industrial quality analytics.

The MVP separates the product into five main layers:

1. User interface
2. Application logic
3. Database
4. File storage
5. AI-assisted analysis

---

## Suggested Architecture

```text
User
 │
 ▼
Next.js Web App
 │
 ├── Authentication
 ├── Configuration UI
 ├── Quality data entry forms
 ├── Dashboards
 └── AI assistant interface
 │
 ▼
Supabase
 │
 ├── Auth
 ├── PostgreSQL database
 └── File storage
 │
 ▼
OpenAI API
 │
 ├── Data interpretation
 ├── Failure mode suggestions
 ├── Root-cause analysis drafts
 ├── Report generation
 └── Consultative assistant
