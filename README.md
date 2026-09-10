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

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

- **[Lakera Guard](https://www.lakera.ai/)**  

  Managed runtime API for real-time prompt-injection, jailbreak, and attack detection with low latency (now part of broader Check Point portfolio).



- **[Protect AI](https://protectai.com/)**  

  AI security platform covering model and supply-chain risk; also the origin of the open-source LLM Guard library.



- **[Aporia](https://www.aporia.com/)**  

  ML and LLM observability/security platform with monitoring and guardrail-style controls for production models.



- **[Portkey AI Gateway](https://portkey.ai/)**  

  AI gateway that includes routing, observability, and guardrail/policy features for LLM traffic.



- **[Fiddler AI](https://www.fiddler.ai/)**  

  Model performance and safety monitoring platform with LLM-focused detection capabilities.



- **[Prompt Security](https://www.prompt.security/)**  

  Runtime protection for GenAI usage, including shadow-AI discovery, DLP, and prompt-injection blocking (now aligned with broader security platforms).



- **[HiddenLayer](https://hiddenlayer.com/)**  

  AI security platform focused on model protection, adversarial detection, and runtime defense.



- **[CalypsoAI](https://calypsoai.com/)**  

  AI security and governance platform offering controls around LLM usage and risk.



- **[Pangea AI Guard](https://pangea.cloud/)**  

  Security services including AI/LLM guard capabilities for content and policy enforcement.



- **[Other commercial LLM firewall & AI security offerings](https://github.com/)**  

  Additional vendors providing managed prompt filtering, red-teaming, or runtime AI defense.



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
