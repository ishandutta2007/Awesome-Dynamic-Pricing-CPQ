# Awesome-Dynamic-Pricing-CPQ

## Top Dynamic Pricing & CPQ Ecosystem

**Curated List of SaaS Platforms & Open-Source GitHub Projects**  
*Focused on Configure-Price-Quote Automation, Price Optimization & Margin Protection*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Dynamic Pricing & CPQ**. These tools help sales and revenue teams configure complex products, apply pricing rules, generate accurate quotes, and enforce discount guardrails—covering everything from Salesforce-native CPQ to AI-driven price optimization engines and open-source billing infrastructure that handles metered pricing.

**Examples** include Salesforce CPQ, DealHub, PROS Smart CPQ, Vendavo, Pricefx, Conga CPQ, Experlogix, and open-source alternatives like Flexprice and Apto.ONE (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted pricing engines, open-source CPQ, and community-driven billing infrastructure—ideal for organizations seeking data sovereignty and avoiding per-seat enterprise licensing. The open-source landscape is genuinely thin for **full CPQ** (Salesforce-native configuration has no open-source equivalent), but functional for **usage-based pricing engines** (Flexprice) and **product configurators** (Apto.ONE). Note that **SwiftCPQ** is the only actively maintained open-source CPQ tool listed on GitHub's `configure-price-quote` topic [citation:2].

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Salesforce CPQ (Revenue Cloud)](https://www.salesforce.com/)** | Enterprise CPQ standard with guided selling, pricing rules, and discount approvals. **Per-seat pricing**: Standard CPQ ~**$75/user/month** list; CPQ Plus ~**$150/user/month** (advanced approvals, amendments, order management). **Billing is priced as a percentage of invoiced volume**—a compounding annuity as revenue grows . | CPQ Standard: ~**$75/user/month** (list); CPQ Plus: ~**$150**; Billing: % of invoiced volume  | No free tier; demo via sales. **Negotiated rates commonly 20–30% below list** with seat audits . |
| **[DealHub](https://dealhub.io/)** | Agentic quote-to-revenue platform covering CPQ, CLM, and Billing. Multi-dimensional pricebooks, usage-based/tiered/hybrid pricing, ramped quotes, co-terminated expansions, and approval-aware pricing. **CRM-agnostic with headless API quoting** [citation:9]. | Quote-only (modular: CPQ, CLM, Billing). Vendr data: 15–30% off list for multi-year . | No free tier; demo via sales. |
| **[PROS Smart CPQ](https://www.pros.com/)** | AI-powered configure-price-quote for complex B2B sales. **Pricing entirely private-offer based via Microsoft Marketplace**—public listings show $0.00 placeholders because PROS quotes custom private offers . | Quote-only (private offers via Microsoft Marketplace) [citation:5][citation:15] | No public free tier; demo via sales. |
| **[Vendavo](https://www.vendavo.com/)** | Pricing, quoting, and rebate management with AI-powered price guidance and margin leak detection. Covers price waterfalls, discount drift, and agreement governance [citation:6]. | Quote-only (enterprise contract) | No free tier; demo via sales. |
| **[Pricefx](https://www.pricefx.com/)** | Three-package offering: **Plan (free analytics)**, Price (AI segmentation), and Profit (CPQ + Velo negotiation). **Plan package is subscription-free**—no recurring payments or time limits for analytics [citation:7]. | **Plan: Free** (analytics); Price/Profit: quote-only  | **Free (Plan)**: subscription-free pricing analytics with Accelerators for CRM/sales data [citation:7] |
| **[Conga CPQ](https://www.conga.com/)** | CPQ within Conga Revenue Lifecycle suite. Software Advice lists starting price at **$85/month** [citation:10]. Frequently positioned for Salesforce-heavy environments. | From **$85/month** (Software Advice) [citation:10] | No free tier; demo via sales. |
| **[Experlogix](https://www.experlogix.com/)** | CPQ for Microsoft Dynamics and Salesforce. Handles complex price tiers, discount stacking rules, and SPA compliance. SelectHub data indicates **~$20,000 annual cost** in some segments [citation:1][citation:8]. | ~**$20,000/year** (SelectHub segment) [citation:1] | No free tier; demo via sales. |
| **[FPX CPQ](https://www.fpx.com/)** | Enterprise CPQ (part of Revalize). Positioned for manufacturers with complex product configuration. | Quote-only (enterprise contract) | No free tier; demo via sales. |
| **[Zoho Pricing](https://www.zoho.com/)** | CPQ/pricing capabilities within the Zoho ecosystem (limited public pricing information available). | Contact Zoho for pricing | Contact vendor |
| **[QuoteWerks](https://www.quotewerks.com/)** | Accessible CPQ for IT solution providers, MSPs, and VARs. **Real-time distributor pricing from 15+ vendors** (Amazon Business, Dell, Cisco, HP, Ingram Micro). **~$14/user/month** [citation:1]. | ~**$14/user/month** [citation:1] | No free tier; trial available |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Flexprice](https://github.com/flexprice/flexprice)** | [![Stars](https://img.shields.io/github/stars/flexprice/flexprice?style=social&color=white)](https://github.com/flexprice/flexprice/stargazers) | **The most mature open-source usage-based pricing and billing infrastructure.** **6,883 stars**, AGPL-3.0. Cloud or self-hosted. Features: **usage metering, credits & top-ups, feature access control**, and support for any pricing model (usage-based, subscription, hybrid). Go backend with React frontend. **Not a CPQ**—it handles the pricing and billing engine layer (metering, invoicing) rather than product configuration and quoting [citation:13]. **Best for developers building usage-based SaaS billing.** |
| **[Apto.ONE](https://github.com/apto-one/apto-one)** | [![Stars](https://img.shields.io/github/stars/apto-one/apto-one?style=social&color=white)](https://github.com/apto-one/apto-one/stargazers) | **Open-source product configurator with guided selling, rules, and live pricing.** Self-hostable (Linux/Windows/macOS or hosting/VM). Features: dependency rules (strict/soft), OnePage and Step-by-Step layouts, **2D/3D product visualization**, prices calculated during configuration (surcharges, discounts, customer-group pricing), quote generation, saved configurations, and translations. **Shopware integration** available; CRM/ERP connectors via provider app stores. **License not specified in listing**—verify before commercial use [citation:12]. **Best for companies with product variants needing guided configuration and pricing.** |
| **[SwiftCPQ](https://github.com/topics/configure-price-quote)** | — | **The only actively maintained open-source CPQ tool on GitHub's `configure-price-quote` topic.** Vue-based, vendor-agnostic proposal tool positioned as an accessible alternative to ConnectWise CPQ, Kaseya Quote Manager, and Scalepad Quoter. Updated **April 2026** [citation:2]. **Exact repository URL not confirmed in search results**—search GitHub topics for "SwiftCPQ" to locate it. **Best for teams wanting a basic open-source CPQ foundation.** |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[flexprice-front](https://github.com/flexprice/flexprice-front)** | — | Frontend for Flexprice (Apache-2.0). React/TypeScript. Self-hosting via Docker or manual npm build. Requires Supabase URL/key and backend API URL [citation:3]. **Pair with the Flexprice backend for a complete self-hosted pricing UI.** |

**Frameworks for building custom systems**: The open-source path to dynamic pricing is **compositional**. **Flexprice** provides the metering and billing engine for usage-based models [citation:13], **Apto.ONE** handles product configuration with rules and live pricing [citation:12], and **SwiftCPQ** offers a basic CPQ proposal foundation [citation:2]. **No open-source project matches Salesforce CPQ's deep CRM integration or PROS's AI-driven price optimization**—expect to build those layers or integrate via APIs.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Dynamic pricing and CPQ platforms handle revenue-critical pricing logic and customer contract data; errors in configuration rules or discount approvals can cause margin loss and customer disputes. Validate all pricing rules against contract terms before production deployment.
- **Pricing transparency varies dramatically in this category.** **Salesforce CPQ** has published list prices (~$75–$150/user/month) but **actual negotiated rates are commonly 20–30% lower** after seat audits and edition right-sizing—CPQ Plus is frequently oversold across entire user bases when only a few power users need it [citation:4][citation:14]. **PROS Smart CPQ** shows $0.00 on Microsoft Marketplace because all pricing is private-offer based [citation:5]. **Pricefx Plan is genuinely free** for analytics with no recurring payments [citation:7]. **Conga CPQ lists $85/month** on Software Advice [citation:10]. **Open-source CPQ is the weakest category**: SwiftCPQ exists but its maturity is unverified ; Apto.ONE is a configurator, not full CPQ, and its license is unspecified ; Flexprice is a billing engine, not CPQ [citation:13]. Validate licensing, feature depth, and integration requirements before committing to any tool for revenue-critical quoting.

---

**Made for revenue operations teams, deal desk analysts, pricing managers, and developers building quote-to-cash infrastructure.**  
Let's make dynamic pricing and CPQ more open, transparent, and margin-safe.
