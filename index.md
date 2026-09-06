---
layout: homepage
---

## About Me

Hi, I'm a Data Scientist and Data Engineer at [BlackRock](https://www.blackrock.com/) in Atlanta, where I work on Aladdin Data — the data platform behind Aladdin, BlackRock's investment and risk platform. I build the engineering layer of data governance: the compliance pipeline that turns policy SQL into per-dataset compliance status, the certification component of Certification-as-a-Service (a Streamlit platform generating PDF certificates), governance agent skills grounded in the internal policy wiki, and the target-state architecture for the enterprise data taxonomy. I lead the firmwide data taxonomy approval forum, and I'm a co-inventor on a patent-pending tokenized data-distribution framework.

Before that I was a research analyst at the University of Georgia, building NLP pipelines over 85K+ news articles and modeling social and economic questions with multilevel models and decomposition methods. I'm also pursuing an MS in Computer Science at Georgia Tech (2027–present).

[Resume (PDF)](assets/files/Huacen_Xu_Resume_2026.pdf)

## Focus Areas

- **Governance Engineering & Automation:** Building the tooling behind enterprise data governance — compliance pipelines, certification automation, taxonomy change management, and AI-grounded agent skills. The patterns are written up in [architecture notes](https://github.com/huacenxu/governance-architecture/blob/main/ARCHITECTURE.md).
- **Agent Evaluation & Applied ML:** LLM agents, retrieval-augmented generation, embedding models and vector search; token-usage and prompt-caching evaluation harnesses; NLP and predictive modeling applied to social and economic questions — peer-reviewed research on moral framing, credit access, and housing disparities.
- **Data Tokenization (US Patent Pending):** Co-inventor on a blockchain-based approach to tokenizing data access entitlements for enterprise data governance, where the token balance is the access control and the ledger is the audit trail.

## Selected Projects

**Governance engineering patterns** — three public repos, one architecture, built on personal time. All data, standards, and names in them are invented.

- **[compliance-pipeline-pattern](https://github.com/huacenxu/compliance-pipeline-pattern)** — Governance policy checks as SQL files, run through a fixed extract → transform → metrics → load pipeline; a new domain is config only, no core code changes.
- **[governance-certification-service](https://github.com/huacenxu/governance-certification-service)** — Turns the pipeline's output into a certificate PDF, walks it through a two-stage approval with HMAC-signed one-click links, and grounds a Q&A assistant on a resilient LLM client (model fallback, error triage, circuit breaker).
- **[policy-knowledge-graph](https://github.com/huacenxu/policy-knowledge-graph)** — Syncs a policy wiki into a deterministic knowledge graph where every edge carries a `why`, routes questions by walking it, and gates the knowledge base with a three-score eval in CI; ships as two Claude Code skills, `ask-governance` and `evaluate-taxonomy`.

**Applied ML**

- **[Bond-Risk-Analyzer](https://github.com/huacenxu/Bond-Risk-Analyzer)** — Decision-tree insights and nearest-neighbor proxy identification to streamline risk analysis for financial datasets.
- **[Embedding-Models-for-AI-Retrieval](https://github.com/huacenxu/Embedding-Models-for-AI-Retrieval)** — Domain-specific embedding model for AI-powered document retrieval: synthetic data generation, fine-tuning, FAISS vector search, evaluated with MRR@5.
- **[PRI-Insights-Chatbot](https://github.com/huacenxu/PRI-Insights-Chatbot)** — ML and LLM-powered question-answering and insight generation for enhanced data interaction.

{% include_relative _includes/publications.md %}

*Full publication list on [Google Scholar](https://scholar.google.com/citations?hl=en&user=Q0wjoTYAAAAJ). Code and projects on [GitHub](https://github.com/huacenxu). [Resume (PDF)](assets/files/Huacen_Xu_Resume_2026.pdf).*
