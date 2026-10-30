<img width="100%" src="./assets/header.svg" alt="Hey, I'm Dolph" />

<div align="center">

<a href="https://nitoriq.com">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1200&color=246FDB&center=true&vCenter=true&width=640&lines=Click+tracking+%C2%B7+attribution+%C2%B7+automation;Server-side+conversions+to+6+ad+platforms;Shopify+orders+matched+back+to+the+click;Built+solo%3A+Nitoriq" alt="Typing SVG" />
</a>

<br/>

<a href="https://nitoriq.com"><img src="https://img.shields.io/badge/Nitoriq-246FDB?style=flat-square&logo=googleanalytics&logoColor=white" alt="Nitoriq" /></a>
<a href="https://byteassembly.dev"><img src="https://img.shields.io/badge/ByteAssembly-0F172A?style=flat-square&logo=codeigniter&logoColor=white" alt="ByteAssembly" /></a>
<a href="https://www.upwork.com/freelancers/~017a1549ad265e5735"><img src="https://img.shields.io/badge/Upwork-Hire%20me-14A800?style=flat-square&logo=upwork&logoColor=white" alt="Upwork" /></a>
<img src="https://komarev.com/ghpvc/?username=Torpedo4007&style=flat-square&color=246FDB&label=Profile+views" alt="Profile views" />

</div>

---

I build the systems that tell marketers which clicks made money. For the past year that has meant designing and shipping **[Nitoriq](https://nitoriq.com)** on my own: a tracking, attribution and automation platform in the same category as Voluum, RedTrack and ClickFlare. I take the same work on for clients: conversion tracking, server-side events, Shopify attribution and the full-stack apps around them.

## Nitoriq

```mermaid
flowchart LR
    A([Ad click]) --> B[Tracking engine<br/>routing · bot & proxy filtering]
    B --> C[Lander → Offer]
    C -->|postback · pixel · Shopify order| D[Attribution<br/>dedupe · click matching]
    F[Cost import<br/>10 ad platforms] --> R
    B --> R[(Reporting store)]
    D --> R
    R --> G[Reports +<br/>AI Copilot · MCP]
    R --> H[Automation<br/>engine]
    D --> I[Conversions API<br/>delivery]
    H --> P([Ad platforms])
    I --> P
```

| Area | What I built |
|---|---|
| **Click tracking** | Redirect and redirectless tracking, custom domains with DNS verification, conditional routing on geo, ASN, device, proxy, bot score, time of day and more (AND/OR, regex), weighted rotation, offer caps |
| **Attribution** | Postback and pixel conversions deduplicated by transaction ID, lander-journey attribution, multi-currency with automatic FX conversion, 20 custom tracking fields |
| **Integrations** | Cost import from Google Ads, Meta, TikTok, Snapchat, Pinterest, Reddit, Taboola, Outbrain, Revcontent, MGID. Server-side conversions to Meta, Google Ads, TikTok, Snapchat, Pinterest, Reddit. Revenue from ClickBank, Everflow, impact.com, Rakuten, Partnerize, AdSense |
| **Shopify** | Embedded app with a Web Pixel and order webhooks. Matches each order back to its click with a confidence score and the evidence behind it, net of refunds |
| **Tag manager** | Versioned containers, GA4 / Meta / Google Ads / TikTok tags, SPA, scroll and visibility triggers, dataLayer support, consent handling, pixel + CAPI dedupe |
| **Automations** | Rules that pause, scale budgets, adjust bids and exclude placements across 7 ad platforms. Every rule can be simulated first and runs behind cooldowns, spend caps and read-back verification |
| **AI Report Copilot** | Reads the report on screen, explains what changed and flags wasted spend. Also exposed to outside AI agents through an MCP server with OAuth and approval-gated writes |
| **Reporting & API** | 3-level drill-down, formula metrics, saved views, shared links. REST API with OpenAPI spec, scoped keys and service principals (RS256 JWT) |

**Engineering choices I'm proud of**

- Redirects never wait on the database. Ingest is async, so a slow write can't slow down an ad click.
- Browser pixels and server-side events share an event ID, so ad platforms count each conversion once.
- Before an automation touches a live campaign, it checks provider health, data freshness and campaign mapping confidence, then reads the change back to confirm it landed.

**Stack:** pnpm monorepo (app, API, docs, help center, Shopify app) · React · TypeScript · Express · PostgreSQL · ClickHouse · Redis · Docker

<a href="https://nitoriq.com"><img src="https://img.shields.io/badge/Visit-nitoriq.com-246FDB?style=for-the-badge" alt="Visit Nitoriq" /></a>

## Work with me

- **Conversion tracking and CAPI:** GTM, GA4, server-side GTM, Meta Conversions API, event matching and deduplication
- **Tracker setup and migration:** Nitoriq, Voluum, RedTrack, ClickFlare, with postbacks, cost import and campaign structure
- **Shopify:** tracking audits, attribution fixes, custom themes, embedded apps
- **Full-stack:** TypeScript, React, Node.js, PostgreSQL, Redis, WordPress, n8n automations

<a href="https://www.upwork.com/freelancers/~017a1549ad265e5735"><img src="https://img.shields.io/badge/Hire%20me%20on-Upwork-14A800?style=for-the-badge&logo=upwork&logoColor=white" alt="Hire me on Upwork" /></a>

## Tools

<p>
  <img src="https://skillicons.dev/icons?i=ts,js,react,nodejs,express,postgres,redis,docker,tailwind,supabase,wordpress,linux&perline=12" alt="Stack" />
</p>
<p>
  <img src="https://img.shields.io/badge/ClickHouse-FFCC01?style=flat-square&logo=clickhouse&logoColor=black" alt="ClickHouse" />
  <img src="https://img.shields.io/badge/Google%20Tag%20Manager-246FDB?style=flat-square&logo=googletagmanager&logoColor=white" alt="Google Tag Manager" />
  <img src="https://img.shields.io/badge/Google%20Analytics%204-E37400?style=flat-square&logo=googleanalytics&logoColor=white" alt="Google Analytics 4" />
  <img src="https://img.shields.io/badge/Meta%20Conversions%20API-0467DF?style=flat-square&logo=meta&logoColor=white" alt="Meta Conversions API" />
  <img src="https://img.shields.io/badge/Shopify-7AB55C?style=flat-square&logo=shopify&logoColor=white" alt="Shopify" />
  <img src="https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white" alt="n8n" />
</p>

<div align="center">

<!-- Snake animation: generated by .github/workflows/snake.yml into the "output" branch -->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Torpedo4007/Torpedo4007/output/github-snake-dark.svg?v=2" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Torpedo4007/Torpedo4007/output/github-snake.svg?v=2" />
  <img alt="Contribution snake" src="https://raw.githubusercontent.com/Torpedo4007/Torpedo4007/output/github-snake.svg?v=2" />
</picture>

</div>

<img width="100%" src="./assets/footer.svg" alt="" />
