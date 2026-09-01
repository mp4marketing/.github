# MP4 Marketing

MP4 Marketing builds and operates the backend systems, integrations, and automations behind the marketing and operations stack for our own agency and the clients we work with.

## What's here

This organization hosts our internal platform and client-specific tooling — mostly Cloudflare Workers, a few Google Apps Scripts, and the shared libraries/services that tie them together.

**Platform & internal tooling**
- [`integrations-gateway`](https://github.com/mp4marketing/integrations-gateway) — OAuth custody (QuickBooks, Google) and ad-platform ingestion connectors (Facebook Marketing, Google Ads)
- [`crm-analytics-hub`](https://github.com/mp4marketing/crm-analytics-hub) — core CRM/analytics backend syncing GHL + ResMan data, AI call analysis, and reporting for our managed clients
- [`ghl-google-ads-conversions`](https://github.com/mp4marketing/ghl-google-ads-conversions) — forwards GHL conversion events to the Google Ads Conversions API for offline attribution
- [`TheEmpireGroupMCP`](https://github.com/mp4marketing/TheEmpireGroupMCP) — MCP server exposing our data warehouse to Claude and other MCP clients
- [`ingestion`](https://github.com/mp4marketing/ingestion) — shared TypeScript library for retry, pagination, and sync primitives used across our Workers
- [`empire-docs`](https://github.com/mp4marketing/empire-docs) — internal documentation site aggregating docs from every project below

**Client-specific**
- [`tw-kpi-sheets-auto-updater`](https://github.com/mp4marketing/tw-kpi-sheets-auto-updater) / [`tw-public-availability-api`](https://github.com/mp4marketing/tw-public-availability-api) — Tower Multifamily reporting and public availability tools
- [`green-empire-analytics-hub`](https://github.com/mp4marketing/green-empire-analytics-hub) / [`green-empire-receipts`](https://github.com/mp4marketing/green-empire-receipts) — Green Empire Landscaping operations and finance automation

## Stack

Cloudflare Workers, D1/Postgres (Supabase), Google Apps Script, and the GoHighLevel/QuickBooks/Google Ads/Databox APIs.

## Status

Most repos here are private and support live production systems for our clients. Public visibility is limited to what's needed for shared tooling.
