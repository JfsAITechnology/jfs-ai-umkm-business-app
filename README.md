# JFS AI UMKM Business App

A reusable multi-tenant UMKM business application under the JFS AI ecosystem.

## Current tenant
- Fibo Laundry

## Architecture target
JFS AI Platform Utama → Authentication → Tenant/Business → UMKM Business App → Database → AI → WhatsApp → Order → Automation

## Design standard
The application follows the JFS AI shared identity:

**[JFS AI Logo] | [Tenant Logo/Name]**

JFS AI is the parent platform/infrastructure. The tenant identity represents the individual UMKM business.

## Current status
Dashboard UI v1 is committed. Backend, Supabase/RLS, real authentication/SSO, tenant data, AI grounding, WhatsApp and order workflows are the next integration stages.

## Security principle
No production secrets are stored in frontend code. AI responses must be grounded in tenant database data and must not invent products, prices, stock, services, promotions or business information.
