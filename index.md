---
layout: homepage
---

## About Me

Hi, I'm a Data Scientist and Data Engineer at [BlackRock](https://www.blackrock.com/) in Atlanta, where I work on Aladdin Data — the data platform behind Aladdin, BlackRock's investment and risk platform. I build the engineering layer of data governance: the compliance pipeline that turns policy SQL into per-dataset compliance status, the certification component of Certification-as-a-Service (a Streamlit platform generating PDF certificates), governance agent skills grounded in the internal policy wiki, and the target-state architecture for the enterprise data taxonomy. I lead the firmwide data taxonomy approval forum, and I'm a co-inventor on a patent-pending tokenized data-distribution framework.

Before that I was a research analyst at the University of Georgia, where I completed an MS in Business Analytics, building NLP pipelines over 85K+ news articles and modeling social and economic questions with multilevel models and decomposition methods.

## Focus Areas

- **Governance Engineering & Automation:** Building the tooling behind enterprise data governance — compliance pipelines, certification automation, taxonomy change management, and AI-grounded agent skills. The patterns are written up in [architecture notes](https://github.com/huacenxu/governance-architecture/blob/main/ARCHITECTURE.md).
- **Agent Evaluation & Applied ML:** LLM agents, retrieval-augmented generation, embedding models and vector search; token-usage and prompt-caching evaluation harnesses; NLP and predictive modeling applied to social and economic questions — peer-reviewed research on moral framing, credit access, and housing disparities.
- **Data Tokenization (US Patent Pending):** Co-inventor on a blockchain-based approach to tokenizing data access entitlements for enterprise data governance, where the token balance is the access control and the ledger is the audit trail.

## Selected Projects

**Governance engineering patterns** — four repos, on sanitized synthetic data.

- **[governance-architecture](https://github.com/huacenxu/governance-architecture/blob/main/ARCHITECTURE.md)** — Architecture notes: where each piece sits on an enterprise data platform, how they connect through the catalog, and what's next, with an at-a-glance diagram.
- **[compliance-pipeline-pattern](https://github.com/huacenxu/compliance-pipeline-pattern)** — Governance policy checks as SQL files, run through a fixed extract → transform → metrics → load pipeline; a new domain is config only, no core code changes.
- **[governance-certification-service](https://github.com/huacenxu/governance-certification-service)** — Turns the pipeline's output into a certificate PDF, walks it through a two-stage approval with HMAC-signed one-click links, and grounds a Q&A assistant on a resilient LLM client (model fallback, error triage, circuit breaker).
- **[policy-knowledge-graph](https://github.com/huacenxu/policy-knowledge-graph)** — Syncs a policy wiki into a deterministic knowledge graph where every edge explains itself, routes questions by walking the graph, and gates the knowledge base with a three-score eval in CI; ships as two Claude Code skills for answering policy questions and evaluating taxonomy changes.

{% include_relative _includes/publications.md %}

*Full publication list on [Google Scholar](https://scholar.google.com/citations?hl=en&user=Q0wjoTYAAAAJ). Code and projects on [GitHub](https://github.com/huacenxu).*
