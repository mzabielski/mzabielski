# Michał Zabielski

**Software engineer & founder · B2B commerce architecture · AI-assisted, spec-driven development**

I design and build B2B sales systems for manufacturers and distributors: commerce platforms, CRMs, and the integrations that connect them to ERP, PIM and WMS. I've been writing code since I was a kid and building e-commerce professionally for 12+ years. Today I run [ENDORA](https://endora.pl) and lead the development of **[Endora Commerce](https://github.com/endora-commerce/endora-commerce)**, an open-source B2B platform.

My niche is where software architecture meets business process: turning messy B2B sales operations (quotes, customer-specific pricing, credit limits, ERP sync) into clean, modular software.

---

## 🛒 Endora Commerce, my main project

[![Repo](https://img.shields.io/badge/endora--commerce-endora--commerce-181717?style=flat&logo=github)](https://github.com/endora-commerce/endora-commerce)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/endora-commerce/endora-commerce/blob/master/LICENSE)
[![npm](https://img.shields.io/npm/v/@endora-commerce/cli?label=npm&logo=npm)](https://www.npmjs.com/package/@endora-commerce/cli)
[![Docs](https://img.shields.io/badge/docs-docs.commerce.endora.software-6322C8)](https://docs.commerce.endora.software)

An open-source B2B and B2C commerce platform where every business capability is a module you can install, switch off or replace. I'm the creator and main contributor.

[![Stars](https://img.shields.io/github/stars/endora-commerce/endora-commerce?style=flat&logo=github&label=stars)](https://github.com/endora-commerce/endora-commerce/stargazers)
[![Forks](https://img.shields.io/github/forks/endora-commerce/endora-commerce?style=flat&logo=github&label=forks)](https://github.com/endora-commerce/endora-commerce/forks)
[![Release](https://img.shields.io/github/v/release/endora-commerce/endora-commerce?style=flat&label=release)](https://github.com/endora-commerce/endora-commerce/releases)
[![Last commit](https://img.shields.io/github/last-commit/endora-commerce/endora-commerce?style=flat&label=last%20commit)](https://github.com/endora-commerce/endora-commerce/commits)
[![Commit activity](https://img.shields.io/github/commit-activity/m/endora-commerce/endora-commerce?style=flat&label=commits)](https://github.com/endora-commerce/endora-commerce/graphs/commit-activity)
[![Contributors](https://img.shields.io/github/contributors/endora-commerce/endora-commerce?style=flat&label=contributors)](https://github.com/endora-commerce/endora-commerce/graphs/contributors)
[![npm downloads](https://img.shields.io/npm/dm/@endora-commerce/cli?style=flat&logo=npm&label=npm%20downloads)](https://www.npmjs.com/package/@endora-commerce/cli)

**By the numbers:** 8,000+ commits of my own · 13 npm packages · 65+ open-source modules · 12 CI workflows · a new release every week

**Architecture**
- **Backend:** Node.js + **Fastify**, **MikroORM** on **PostgreSQL**, Redis, Meilisearch
- **Admin:** React, with a permissioned admin shell, a page and e-mail builder, and a ⌘K command palette with an AI assistant
- **Storefront:** server-rendered **Next.js** and PWA, generated as a standalone app that the merchant owns
- **pnpm monorepo** of publishable packages: `platform`, `modules`, `contracts`, `admin-kit`, `page-builder-core`, `llm-client`, `test-kit`, a CLI and a `create-endora-commerce` installer
- **Deployment:** Docker / Compose; API, admin and storefront can run on one host or on separate machines

**B2B domain, built in:** customer organisations with roles and credit limits, organisation pricing, RFQs and quotes, quick order, shopping lists, multi-tenant / multi-channel / multi-currency, plus vendor-neutral payment, shipment, ERP and PIM connector layers that third parties can write adapters for.

**How it's built**
- 📐 **Spec-Driven Development:** every feature starts as a written specification (`specs/`, Spec Kit) before any code
- 🤖 **AI agents as developers:** most of the code is written by AI coding agents (Claude Code, Codex, Cursor), guided by specs and repo-level agent instructions, then reviewed and gated by humans and CI
- ✅ **Quality gates in CI:** backend test suite, public acceptance tests, boot and pack gates, storefront build, Lighthouse, Changesets-based releases to npm, DCO
- 🔒 **Security:** a security policy and regular white-box audits of the open core and the paid modules
- 🧩 **Open core:** MIT core, with commercial modules (payment gateways, couriers, ERP/PIM sync, Polish KSeF e-invoicing) behind the same public interfaces

```bash
npx create-endora-commerce@latest my-shop
cd my-shop && pnpm run dev:all
```

---

## 📈 GitHub activity

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-activity-graph.vercel.app/graph?username=mzabielski&theme=github-compact&hide_border=true&area=true">
    <img alt="Contribution activity graph" src="https://github-readme-activity-graph.vercel.app/graph?username=mzabielski&theme=minimal&hide_border=true&area=true">
  </picture>
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com?user=mzabielski&theme=github-dark-blue&hide_border=true">
    <img alt="GitHub streak stats" src="https://streak-stats.demolab.com?user=mzabielski&hide_border=true">
  </picture>
</p>

---

## 🔌 What I work on

| Area | Details |
| --- | --- |
| **B2B commerce platforms** | Endora Commerce, Magento / Adobe Commerce, Shopware, Sylius, PrestaShop, WooCommerce |
| **Integrations** | ERP (SAP, Comarch XL, enova365, Symfonia, Subiekt GT), PIM (Pimcore, Akeneo, Ergonode), CRM (HubSpot, Pipedrive, Livespace), WMS / OMS |
| **Custom software** | Dedicated CRMs for B2B sales teams, PWAs, internal tools |
| **Data & AI** | LLM-based features and agents, analytics and BI (Power BI, Looker Studio, Qlik, Streamlit) |
| **Architecture & consulting** | Platform selection, technical audits, integration architecture, build-vs-buy decisions |

---

## 🛠️ Tech stack

**Now:**
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)
![Fastify](https://img.shields.io/badge/Fastify-000000?style=flat&logo=fastify&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![Meilisearch](https://img.shields.io/badge/Meilisearch-FF5CAA?style=flat&logo=meilisearch&logoColor=white)
![pnpm](https://img.shields.io/badge/pnpm-F69220?style=flat&logo=pnpm&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
![Claude Code](https://img.shields.io/badge/Claude_Code-D97757?style=flat&logo=anthropic&logoColor=white)

**Also:**
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat&logo=php&logoColor=white)
![Symfony](https://img.shields.io/badge/Symfony-000000?style=flat&logo=symfony&logoColor=white)
![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=flat&logo=laravel&logoColor=white)
![Magento](https://img.shields.io/badge/Magento-EE672F?style=flat&logo=magento&logoColor=white)
![Shopware](https://img.shields.io/badge/Shopware-189EFF?style=flat&logo=shopware&logoColor=white)
![Sylius](https://img.shields.io/badge/Sylius-1A9F83?style=flat&logo=sylius&logoColor=white)
![Medusa.js](https://img.shields.io/badge/Medusa.js-000000?style=flat&logo=medusa&logoColor=white)
![PrestaShop](https://img.shields.io/badge/PrestaShop-DF0067?style=flat&logo=prestashop&logoColor=white)
![WooCommerce](https://img.shields.io/badge/WooCommerce-96588A?style=flat&logo=woocommerce&logoColor=white)
![Open Mercato](https://img.shields.io/badge/Open_Mercato-1F2937?style=flat)
![Pimcore](https://img.shields.io/badge/Pimcore-6428B4?style=flat&logo=pimcore&logoColor=white)
![Akeneo](https://img.shields.io/badge/Akeneo-9452BA?style=flat)
![UnoPIM](https://img.shields.io/badge/UnoPIM-0041FF?style=flat)
![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat&logo=vuedotjs&logoColor=white)
![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat&logo=react&logoColor=61DAFB)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat&logo=powerbi&logoColor=black)

---

## 🧭 Background

- **2013:** started as a web developer at an e-commerce software house in Warsaw and founded **ENDORA**
- **2013–2017:** PhD studies at the Military University of Technology (WAT), teaching Graph & Network Theory and Web 2.0
- **2017:** co-created **MergeBit Analyzer**, a web analytics tool for e-commerce with an AI engine
- **2013–today:** 120+ delivered projects at Endora for clients in 5 countries, mostly manufacturing, automotive parts, technical distribution and wholesale
- **2026:** started Endora Commerce, using AI agents and spec-driven development to turn 12+ years of B2B know-how into an open-source product

I also host **[Manufaktura e-commerce](https://open.spotify.com/show/4q8gC1FjpHLAmCjYAkrK8P)**, a Polish podcast about e-commerce, and write at [michalzabielski.pl](https://michalzabielski.pl/blog).

---

## 📫 Contact

Working on a B2B platform, an ERP integration, or wondering whether to build or buy? Get in touch.

[![Website](https://img.shields.io/badge/michalzabielski.pl-6322C8?style=for-the-badge&logo=googlechrome&logoColor=white)](https://michalzabielski.pl)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mzabielskipl)
[![Discord](https://img.shields.io/badge/Endora_Commerce-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/GJ2Yk9CvY)
[![X](https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/MZabielskiPL)
