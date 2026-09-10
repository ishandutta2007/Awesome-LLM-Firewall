# Awesome-LLM-Firewall

## Top LLM Firewall / Guardrails Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Prompt Injection Defense, Jailbreak Detection, Input/Output Filtering, Policy Enforcement & AI Runtime Security*

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **LLM Firewalls and Guardrails**. These systems inspect prompts and responses in real time to block prompt injection, jailbreaks, toxic content, data leakage, and policy violations before they reach users or downstream systems.



**Examples** include Lakera Guard, NVIDIA NeMo Guardrails, Protect AI, Aporia, Portkey AI Gateway, Fiddler AI, Prompt Security, HiddenLayer, CalypsoAI, and Pangea AI Guard (the category leaders).



**Open-source emphasis**: LLM guardrails have strong open options. **NVIDIA NeMo Guardrails**, **LLM Guard**, **Guardrails AI**, **LlamaFirewall**, and related projects provide programmable, self-hostable protection. This section is heavily expanded with these tools.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saashosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

| Platform / Product | Description / Focus | Pricing (Starting Tier) | Free Tier Limits / Free Trial |
| :--- | :--- | :--- | :--- |
| **[Lakera Guard](https://www.lakera.ai/)** | Managed runtime API for real-time prompt-injection, jailbreak, and DLP detection with low latency (now part of Check Point portfolio). | **Community:** $0/mo<br>**Enterprise:** Starts at ~$50,000/year (custom contract via AWS Marketplace / Sales) | **Free Forever (Community Plan):** 10,000 API requests/month with full prompt injection, jailbreak, and DLP detection + dashboard reporting. |
| **[Portkey AI Gateway](https://portkey.ai/)** | Production AI Gateway with guardrail policy enforcement, multi-LLM routing, fallbacks, load balancing, and observability. | **Developer:** $0/mo<br>**Production:** Starts at $49/month (includes 100,000 recorded logs)<br>**Enterprise:** Custom quotes | **Free Forever (Developer Plan):** 10,000 recorded logs/month (traffic continues unblocked beyond limit), 3-day log retention, 30-day metrics, 3 prompt templates. |
| **[Pangea AI Guard](https://pangea.cloud/)** | API-first security services providing AI Guard for prompt injection defense, sensitive data redaction, and policy enforcement. | **Pay-As-You-Go:** Starts at $0.001 per request ($1.00 / 1,000 requests) or $0.0001 per scanned token<br>**Enterprise Credits:** Starts at $500 minimum commitment | **Free Forever Account:** $5/month complimentary usage credit (~5,000 requests/month) with standard API rate limits (100 req/day burst during development). |
| **[Fiddler AI](https://www.fiddler.ai/)** | Model safety & monitoring platform offering real-time guardrails (<80ms latency for safety/PII/injection) and GenAI observability. | **Free Guardrails:** $0/mo<br>**Developer (Observability):** $0.002 per trace<br>**Enterprise:** Custom quote-based annual contracts | **Free Forever Plan:** Unlimited real-time guardrail filtering (prompt injection, jailbreak, PII/PHI, toxicity; excludes trace storage)<br>**14-day Free Trial** for full observability suite. |
| **[Aporia](https://www.aporia.com/)** | Real-time LLM guardrails (hallucination mitigation, toxic content, data leakage) and ML observability (now part of Coralogix). | **Starter / Team:** Starts at ~$1,000/month (~$12,000/year)<br>**Enterprise:** Custom scale-based contracts | **14-day Free Trial:** Full platform access including real-time guardrails, monitoring, and up to 10,000 prediction/evaluation requests. |
| **[Protect AI](https://protectai.com/)** | AI-SPM platform covering ML model security scanning (Guardian/Radar) and runtime AI risk; origin of open-source LLM Guard. | **Enterprise Platform:** Starts at ~$25,000/year (AWS Marketplace contract)<br>**LLM Guard Library:** Free & open-source (MIT) | **14-day Guided Proof-of-Concept / Trial:** Scoped to 5 models or 50,000 scanned requests<br>**Unlimited free self-hosted usage** via open-source LLM Guard library. |
| **[Prompt Security](https://www.prompt.security/)** | Runtime GenAI firewall, shadow-AI discovery, DLP, and prompt injection defense (integrated into SentinelOne Singularity). | **Enterprise Contract:** Starts at ~$15,000/year (per-seat / workload licensing via SentinelOne) | **14-day to 30-day Proof-of-Concept Sandbox:** Evaluation access for up to 100 employee seats / 25,000 prompt inspections. |
| **[HiddenLayer](https://hiddenlayer.com/)** | AISec platform providing ML/LLM model scanning, adversarial attack defense, and runtime firewalling. | **AISec Platform:** Starts at ~$20,000/year (AWS/Azure Marketplace unit-based contract licensing) | **30-day Enterprise Proof-of-Value (POV):** Full runtime & scanning evaluation for up to 2 production models upon sales qualification. |
| **[CalypsoAI](https://calypsoai.com/)** | Enterprise AI security and governance (Moderator platform) for policy enforcement, DLP, and prompt firewalling (via F5). | **Enterprise Subscription:** Starts at ~$30,000/year (custom enterprise contract via F5) | **14-day Evaluation Sandbox:** Hands-on demo sandbox access with full policy configuration and up to 5,000 test prompt evaluations. |




## Open-Source GitHub Projects

- **[NVIDIA NeMo Guardrails](https://github.com/NVIDIA/NeMo-Guardrails)**  

  Leading open-source toolkit for programmable guardrails — Colang-based dialog flows, input/output rails, jailbreak detection, topic control, and safety checks. Fully self-hostable.



- **[LLM Guard (Protect AI)](https://github.com/protectai/llm-guard)**  

  Open-source (MIT) Python library for scanning prompts and outputs — prompt injection, toxicity, PII, secrets, and more. Runs entirely on your infrastructure.



- **[Guardrails AI](https://github.com/guardrails-ai/guardrails)**  

  Open-source framework for validating and structuring LLM inputs/outputs with a rich set of validators (PII, toxicity, schema, etc.).



- **[LlamaFirewall (Meta)](https://ai.meta.com/research/publications/llamafirewall-an-open-source-guardrail-system-for-building-secure-ai-agents/)**  

  Open-source guardrail system focused on agent security — prompt injection detection (PromptGuard), alignment checks, and code safety.



- **[Rebuff and similar injection defenses](https://github.com/)**  

  Community projects specifically targeting prompt-injection detection and canary-based defenses.



- **[garak (NVIDIA)](https://github.com/NVIDIA/garak)**  

  Open-source LLM vulnerability scanner / red-teaming tool for probing models and applications before production.



- **[Open policy and moderation models](https://github.com/)**  

  Llama Guard, NVIDIA safety models, and other open classifiers that can be wired into custom firewall pipelines.



- **[Custom Colang / policy engines](https://github.com/)**  

  Extensions and examples built on NeMo Guardrails for domain-specific rails and multi-agent safety.



- **[PII and secrets scanning open libraries](https://github.com/)**  

  Standalone detectors often composed into broader LLM firewall stacks.



- **[Gateway + filter open proxies](https://github.com/)**  

  Lightweight open proxies that apply regex, classifier, or LLM-based filters before forwarding requests to model providers.



### Additional Strong Open-Source Options

- Deploying **NeMo Guardrails** when you need programmable conversation flows and deep policy control.

- Using **LLM Guard** or **Guardrails AI** for fast, library-style input/output scanning with full data privacy.

- Combining **LlamaFirewall**-style agent checks with broader application guardrails for multi-agent systems.

- Running **garak** regularly in CI to red-team prompts and configurations.

- Layering open classifiers (toxicity, injection, PII) in front of any LLM endpoint.

- Accepting that managed low-latency APIs, large proprietary attack datasets, and enterprise support still favor commercial services like Lakera for some teams.



**Frameworks for building custom systems**: Intercept every prompt and completion → run open scanners (LLM Guard / Guardrails AI / NeMo rails) → block or rewrite unsafe content → log decisions for audit. Add red-teaming with garak. This stack keeps data on-prem and is highly customizable. Commercial platforms (Lakera Guard, Protect AI, Prompt Security, HiddenLayer, etc.) remain strong when you want a managed, low-latency API or broader AI security posture management without operating the detectors yourself.



## How to Contribute

1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.

- LLM firewalls reduce risk but do not eliminate it. Prompt injection and jailbreak techniques evolve quickly; no guardrail is perfect. Always combine technical controls with secure application design, least-privilege tool access, human oversight for high-stakes actions, and regular red-teaming. Open-source deployments require proper model hosting, latency testing, and policy maintenance. This list is not security or compliance advice.



---

**Made for AI security engineers, platform teams, and builders who refuse to ship unguarded LLM applications.**

Let's keep AI interactions safer, auditable, and under explicit policy control.
