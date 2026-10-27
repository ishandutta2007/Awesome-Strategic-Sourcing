# Awesome-Strategic-Sourcing

## Top Strategic Sourcing Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Sourcing Optimization, RFQ Automation & Supplier Award Decisions*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Strategic Sourcing**. These tools enable procurement teams to identify savings opportunities, run competitive bidding events, evaluate suppliers against multiple criteria, and award contracts—moving beyond tactical purchasing to data-driven sourcing decisions that balance cost, risk, quality, and sustainability.



**Examples** include Workday Strategic Sourcing, Coupa, SAP Ariba, Keelvar, Scout RFP, Ivalua, Jaggaer, Fairmarkit, GEP SMART, and Sievo (the category leaders).



**Open-source emphasis**: Strategic Sourcing is a domain where open-source tooling is **emerging but fragmented**. The strongest active project is **mcp-procurement** (zavora-ai), which provides a comprehensive source-to-pay backbone with RFQ creation, quote comparison, price benchmarking, supplier scoring, and negotiation briefs. Other projects focus on RFQ workflow (VendSync, BidForge) or sourcing intelligence analytics (aribaiq, aribacortex) but lack the full optimization and award-decision depth of dedicated strategic sourcing platforms. Organizations requiring advanced sourcing optimization (Keelvar-style scenario modeling) should plan for commercial platforms.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Workday Strategic Sourcing](https://www.workday.com/)**  

  Strategic sourcing within Workday's spend management suite, covering sourcing events, RFx management, bid comparison, and award workflows integrated with supplier and contract data.



- **[Coupa](https://www.coupa.com/)**  

  Sourcing module within Coupa's spend management platform; supports RFx creation, supplier bidding, side-by-side comparison, and award decisions with category strategy integration.



- **[SAP Ariba](https://www.sap.com/)**  

  Comprehensive sourcing suite with RFx, reverse auctions, supplier qualification, and award optimization; integrates with Ariba Network for supplier discovery and bidding.



- **[Keelvar](https://www.keelvar.com/)**  

  AI-driven sourcing optimization platform with powerful scenario optimization engine for "what-if" analyses, automation bots for recurring events, and simultaneous evaluation of multiple supplier constraints and risk variables; best-in-class for complex large-scale sourcing with multi-variable optimization.



- **[Scout RFP (Workday)](https://www.workday.com/)**  

  Strategic sourcing platform with API-driven event management, bid line items, award management, and supplier contact management; integrated into Workday's spend management ecosystem.



- **[Ivalua](https://www.ivalua.com/)**  

  Source-to-Contract solution with AI-powered Intake Management and sourcing workflows; includes intelligent agents for supplier analysis and conversational analytics.



- **[Jaggaer](https://www.jaggaer.com/)**  

  Spend management suite with RFx template import, conditional assessment rules, automated supplier gating, and sourcing event management for direct and indirect procurement.



- **[Fairmarkit](https://www.fairmarkit.com/)**  

  Automated sourcing platform for tail spend and below-threshold purchases; buyers create events, receive AI-recommended supplier suggestions, and compare responses side-by-side.



- **[GEP SMART](https://www.gep.com/)**  

  AI-powered source-to-pay software with RFx and e-auction management with auto-scoring, contract lifecycle management, and supplier performance dashboards.



- **[Sievo](https://sievo.com/)**  

  Procurement analytics platform with spend classification, savings tracking, and sourcing opportunity identification to inform strategic sourcing decisions.



## Open-Source GitHub Projects



- **[mcp-procurement (zavora-ai)](https://github.com/zavora-ai/mcp-procurement)**  

  The most comprehensive open-source sourcing backbone available (v1.1.0); provides **37 MCP tools** covering the full source-to-pay lifecycle including RFQ creation, supplier response, quote comparison with automatic price intelligence, and purchase order generation . Key sourcing-relevant tools include `rfq_create`, `rfq_respond`, `rfq_compare` for side-by-side bid evaluation, `price_benchmark` comparing quotes against historical averages with verdicts and recommendations, `supplier_recommend` for AI-ranked supplier suggestions, `supplier_risk_score` for multi-factor risk assessment (country, performance, contracts, rating), and `negotiation_brief` generating leverage analysis, BATNA, talking points, and strategy . Also includes `savings_opportunity` to find same SKU at different prices across suppliers, `maverick_spend_detect` for purchases outside contracted suppliers, and `supplier_scorecard` with A/B/C/D grading . Designed as an MCP server for AI agents rather than a standalone web application.



- **[VendSync (BidFlow)](https://github.com/RavalMunjal/VendSync)**  

  Full-stack procurement and vendor management ERP (React/Node.js/MongoDB) with structured RFQ management and quotation comparison workflows . Features vendor portal for independent quotation submission, side-by-side comparison with lowest-price auto-highlighting, structured approval workflows with remarks, auto-generated purchase orders from accepted quotes, and real-time analytics dashboards . **RFQ-focused**—provides the bidding workflow and comparison matrix but lacks advanced sourcing optimization (scenario modeling, multi-variable award optimization) and supplier intelligence analytics.



- **[BidForge](https://github.com/tan1ro/BidForge)**  

  Full-stack RFQ platform with **British Auction-style bidding** (dynamic time extensions, real-time updates via WebSocket); features one active bid per bidder per RFQ with immutable revision history, deterministic rank calculation by lowest total bid, auto-extension for British-style auctions, RFQ award workflow after close, and metrics dashboards with optional AI recommendations . Tech stack: FastAPI, MongoDB, React, MUI . **Auction-focused**—excels at competitive bidding mechanics but lacks supplier qualification, spend analytics, and sourcing optimization capabilities.



- **[aribaiq](https://pypi.org/project/aribaiq/)**  

  Open-source Python library for AI-powered procurement and **sourcing intelligence analytics** . Features supplier intelligence scoring (on-time rate, defect rate, ESG score, spend concentration), spend analytics highlighting category concentration and consolidation opportunities, ESG-weighted evaluation, responsible AI checks (missingness, invalid values, representation imbalance), and GenAI-ready prompt generation for copilots and LLM workflows . CLI included for running analytics on CSV/JSON/JSONL files . **Analytics-focused**—provides sourcing intelligence but not the RFQ/auction execution workflow.



- **[aribacortex](https://pypi.org/project/aribacortex/)**  

  Open-source SAP Ariba Procurement Intelligence and **Sourcing Analytics** toolkit (MIT) . Features supplier intelligence scoring (cost, delivery, quality, risk, ESG, compliance), spend optimization insights, procurement risk analytics including single-source exposure detection, ESG-aware supplier evaluation, predictive sourcing foundation with ML-ready scoring, and P2P workflow insights (touchless rate, exception rate, cycle time) . CLI and Python API available . **SAP Ariba-focused analytics**—useful for teams in Ariba environments but not a standalone sourcing execution platform.



- **[OpenTradeIntel](https://pypi.org/project/opentradeintel/)**  

  Open-source procurement and B2B **sourcing intelligence engine** that queries EU public procurement notices from the TED Search API, normalizes them into typed tenders, and ranks them against a local supplier catalog with deterministic 0–100 matching scores . Includes Typer CLI, FastAPI API, and MCP adapter; fully local and offline-capable for core features . **Tender discovery-focused**—useful for identifying public sector sourcing opportunities but not for running private RFx events or supplier award optimization.



### Additional Strong Open-Source Options



- **GitHub `sourcing` or `procurement` topics** — Community repositories focus on RFQ workflow tools (VendSync, BidForge), procurement analytics libraries (aribaiq, aribacortex), or source-to-pay platforms (OpenS2P). No mature open-source equivalent to Keelvar's optimization engine or Coupa's full sourcing suite exists.

- **OpenS2P** — AI-native open-source Source-to-Pay platform (hackathon project) with purchase requisitions, supplier management, and multi-tenant architecture; roadmap includes sourcing and contracting features but current capabilities are foundational .



**Frameworks for building custom systems**: **mcp-procurement** provides the broadest sourcing intelligence foundation with RFQ comparison, price benchmarking, supplier risk scoring, and negotiation briefs—but requires an MCP client for interaction. **VendSync** or **BidForge** can serve as RFQ execution layers (bidding workflow, quote comparison, award). **aribaiq** or **aribacortex** provide sourcing analytics and supplier scoring but not execution. A complete strategic sourcing system would require integrating RFQ execution (VendSync/BidForge) with sourcing intelligence (mcp-procurement/aribaiq) and custom development for advanced optimization—a substantial engineering effort with no single open-source platform providing the full stack.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Strategic sourcing platforms handling supplier bids and contract awards must comply with applicable procurement regulations, anti-corruption laws, and organizational governance policies; bid confidentiality and audit trails are critical.

- **Open-source strategic sourcing remains fragmented**—mcp-procurement provides sourcing intelligence and RFQ tools but as an MCP server; VendSync and BidForge provide RFQ execution but lack optimization; aribaiq and aribacortex provide analytics but not execution. No open-source platform matches Keelvar's multi-variable optimization or Coupa's integrated sourcing suite. Organizations requiring advanced sourcing optimization should plan for commercial platforms.

- Verify license terms for commercial use; mcp-procurement is an open-source MCP server , VendSync is a hackathon project , BidForge is open-source , and aribaiq/aribacortex use MIT .



---



**Made for sourcing managers, procurement analysts, category managers, and supply chain strategists.**  

Let's make strategic sourcing more open, data-driven, and award-optimized.
