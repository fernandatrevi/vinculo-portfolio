# Vínculo | Technical Case Study

## 1. Problem and motivation

Nonprofit organizations may need to manage campaigns, donor records, and follow-up activities across different processes. Vínculo explores connecting public project discovery with administrative tools. This is a **design motivation**, not a measured finding from participating nonprofits.

## 2. Value proposition

Provide a public nonprofit directory alongside permission-controlled management tools. A longer-term goal is to connect recorded donations to acknowledgment and follow-up workflows, subject to further development and validation.

## 3. Current functionality

| Component | Documented implementation |
|---|---|
| Public directory | Three fictional nonprofit profiles with filters and project descriptions |
| Registration and access | API-based account registration, login, logout and account retrieval |
| Memberships | Retrieve affiliated organizations; no automatic organization access |
| Administrative records | Permission-controlled manual donor and donation record operations in PostgreSQL |
| Sample dashboard | Fictional data and some actions stored in browser localStorage |
| Sample follow-ups | Local simulation, not persistent multi-user collaboration |
| Online payments | Not implemented |
| Email verification | Not implemented |
| Recurring payments, notifications, verified reports | Pending |

Local test results do not establish comprehensive production deployment validation.

## 4. Tools and engineering capabilities

- React, TypeScript and Vite for the web application
- FastAPI and Pydantic for backend endpoints
- PostgreSQL and SQL migrations for structured persistence
- Authentication and membership-based access control
- Render for separately hosted web interface and API

## 5. Example user journey

1. A visitor browses the public directory.
2. A visitor registers using fictional data for demonstration.
3. The user signs in and views their account.
4. Without an assigned membership, the user cannot administer an organization.
5. Some administrative operations require specific permissions, while the sample dashboard is not a shared production system.

## 6. Potential business indicators — not measured project outcomes

A future product might track confirmed donation amounts, recurring donor rates, acknowledgment time, donor retention and follow-up completion. Doing so would require reliable input records, unambiguous metric definitions and financial reconciliation.

## 7. Limitations and next steps

- Avoid processing real donor information until appropriate security and privacy safeguards are validated.
- Add email verification and automated tests for critical workflows.
- Resolve existing linting issues and verify permissions in the deployed environment.
- Develop accounting reconciliation before claiming payment collection.
- Define data handling and operational procedures.
- Validate proposed impact metrics through appropriately scoped pilots.

## 8. Technical learning outcomes

Vínculo supports discussions of data modeling, frontend/backend integration, relational persistence, role-based access and the difference between prototype functionality and production systems.

**[Open the demonstration](https://vinculo-donantes-1.onrender.com/)** — the free hosting service may need to start after inactivity.

*No private application source code is included in this case study.*
