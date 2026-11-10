# Vínculo — Social Impact & Nonprofit Management

**Public portfolio · Full-stack web prototype · Technology for social impact**

[**Explore the live demo**](https://vinculo-donantes-1.onrender.com/) · [Case study](docs/CASE_STUDY.md) · [Architecture](docs/ARCHITECTURE.md) · [Interview guide](docs/INTERVIEW.md)

> **Private source code.** This repository only contains a public presentation of the project, not the application's frontend, backend, migrations, credentials, or donor information.

## Overview

Vínculo is an **early-stage full-stack prototype** exploring how nonprofit organizations could connect with supporters while organizing administrative workflows related to donors and donations.

The project combines a public directory, user accounts, organization memberships and permission-controlled record management.

**Current status:** experimental demonstration using fictional information. **It does not collect payments, process credit cards, or support production use with real donor information.** Manually recording a donation is not equivalent to processing a financial transaction.

## Documented features

| Module | Current scope |
|---|---|
| Public directory | Three fictional nonprofit profiles, filters and project descriptions |
| User accounts | API-based registration, sign-in, account retrieval and sign-out |
| Organization memberships | Retrieve the organizations associated with an account |
| Donor and donation records | Manual create, read and update operations, subject to permissions |
| Sample dashboard | Fictional data; some interactions are stored only in the browser |
| Sample follow-ups | Local demonstration, not a shared multi-user workflow |
| Payments, email verification and verified reports | Not implemented or not yet validated |

New accounts do not automatically receive organization administration rights.

## Technology stack

- **Frontend:** React, TypeScript, Vite
- **Backend:** Python, FastAPI, Pydantic
- **Data storage:** PostgreSQL, versioned SQL migrations
- **Access:** sessions, memberships, permission controls and password hashing
- **Hosting:** Render, with separate frontend, API and database resources

## Conceptual data flow

```text
Organizations and projects → Public directory
User account → Authentication → Memberships and permissions
Authorized management → API → PostgreSQL
Sample dashboard → Fictional browser-local data
```

## Live demonstration

**[Open Vínculo on Render](https://vinculo-donantes-1.onrender.com/)**

Select **“Ver panel de ejemplo” (View sample dashboard)** to explore the demo. Use only fictional information. The hosted service may require time to start after inactivity; availability has not been independently verified.

## What this project demonstrates

- Translating a social-sector problem into a full-stack product concept
- Connecting a web interface, API and relational database
- Structuring account, membership and access-control workflows
- Separating persisted operational records from demonstration-only data
- Documenting implementation gaps, data-quality concerns and technical trade-offs

## Scope and responsible use

Vínculo is a **prototype**, not a production-ready payment or donor management platform. End-to-end permissions, privacy safeguards and workflows require validation before any real-world deployment. Do not enter actual donor information or personal credentials into the demo.

## Project documentation

- [Technical case study](docs/CASE_STUDY.md)
- [Architecture and privacy boundaries](docs/ARCHITECTURE.md)
- [Interview talking points](docs/INTERVIEW.md)
- [Portfolio landing page](index.html)

**Portfolio project by Fernanda Treviño.** The application's source repository remains private.
