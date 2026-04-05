# HarborPSH

**HIPAA-compliant operations platform for California's permanent supportive housing providers.**

> Replacing spreadsheets, disconnected portals, and manual compliance tracking with a single platform purpose-built for PSH workflows.

---

## The Problem

California has 180,000+ people in permanent supportive housing programs, backed by $3.3B in annual state funding. The nonprofit providers running these programs manage vulnerable populations with life-critical services — but most still operate on spreadsheets, paper files, and disconnected systems.

- **72% of PSH providers** use spreadsheets for tenant tracking
- **40+ hours/month** wasted on manual HUD reporting
- **HIPAA exposure** from sensitive health data in unencrypted emails and shared drives
- **One missed compliance deadline** can jeopardize funding for an entire program

## The Solution

HarborPSH is a single, HIPAA-compliant platform covering the full operational lifecycle of permanent supportive housing:

| Module | What It Does |
|---|---|
| **Tenant Management** | Intake through transition — demographics, unit assignments, lease compliance, recertification scheduling |
| **Case Coordination** | HIPAA-compliant case notes, service plans, and care team collaboration with AI-powered summaries |
| **Compliance Engine** | Automated tracking for HUD reporting, HMIS data, HQS inspections, and annual recertifications |
| **AI Assistant** | Natural language queries across your portfolio — "Which tenants have recertifications due this month?" |

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | Next.js 14, React, Tailwind CSS, shadcn/ui |
| Backend | Supabase (PostgreSQL), Row-Level Security |
| AI | Google Gemini streaming chat |
| Auth | NextAuth.js with Azure AD (HIPAA-ready) |
| Hosting | Vercel (SFO1 region), Google Cloud Run |
| CI/CD | GitHub Actions — 5-stage pipeline (lint → test → build → deploy → health check) |
| Monitoring | Sentry error tracking with release notifications |
| Security | AES-256 encryption, RLS policies, SOC 2 ready |

## Database Schema

9-table PostgreSQL schema covering:

- `tenants` — Demographics, contact info, status
- `units` — Property and unit inventory
- `leases` — Lease terms, rent calculations, recertification dates
- `case_notes` — HIPAA-compliant clinical and service notes
- `service_plans` — Individualized service plans with goals and milestones
- `inspections` — HQS inspection tracking and scheduling
- `compliance_events` — Audit trail for all compliance-related activities
- `staff` — Case workers, property managers, admin roles
- `documents` — Secure document storage with access controls

All tables enforce Row-Level Security (RLS) policies to ensure tenant data isolation.

## Target Market

**Primary:** California nonprofit PSH operators managing 50–500 units

**Expansion:** National PSH market (3,000+ providers), transitional housing, rapid rehousing programs

**Pricing:** SaaS subscription — per-unit/month model aligned with how providers budget

## Founder

**Michelle Davis** — Solo Founder & CEO, MD Development

- Background in event coordination and nonprofit operations, including the Path Forward Initiative in San Bernardino
- AI-native builder running a venture studio from Riverside County, CA
- Designs, architects, and ships production B2B SaaS using conversational AI workflows
- HarborPSH is part of a portfolio of deployed products including CalibrationFlow AI and ReLoop Asset Stream

## Status

- ✅ Full Next.js + Supabase + Tailwind production scaffold
- ✅ 9-table database schema with RLS policies
- ✅ Gemini streaming AI chat integration
- ✅ CI/CD pipeline via GitHub Actions
- ✅ Vercel deployment config (SFO1 region)
- ✅ Sentry error monitoring
- ✅ Investor one-pager and funding materials
- 🔲 Pilot onboarding with first PSH provider
- 🔲 Custom domain (harborpsh.com)
- 🔲 HIPAA BAA execution with Supabase

## Links

- **Landing Page:** [Coming soon]
- **Studio:** [MD Development](https://github.com/MDavis-byte)
- **LinkedIn:** [Michelle Davis](https://linkedin.com/in/reloopassetstream)

## License

Proprietary — © 2026 MD Development. All rights reserved.
