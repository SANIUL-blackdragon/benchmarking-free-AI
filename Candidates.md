# Benchmarking-Free-AI Candidates.md

## Introduction
This document serves as the central candidate list for benchmarking fully free AI models accessible via their official websites. As of 05:39 PM +06 on Monday, October 20, 2025, candidates are selected based on strict criteria: 
- **100% free access**: No payments, subscriptions, or hidden fees for core functionality.
- **No limits**: Unlimited prompts/queries without daily/hourly caps, rate throttling, or usage tiers (e.g., no "20 messages/day" or "wait 24 hours for recharge").
- **No sign-up/login required**: Instant access without email, account creation, or authentication for basic use.
- **Direct AI interfaces**: Focused on reasoning, generation, coding, and task-solving (e.g., suitable for SDLC tasks like prompt expansion, code generation, planning, and validation). Excludes roleplay/character chats (e.g., no Perchance AI RP, Gening AI, or Character.AI alternatives from Reddit discussions).
- **Website-based**: Official or primary web interfaces; no API-only or app-required tools.

The list is curated from verified sources (e.g., official docs, 2025 reviews on Medium/DataCamp, Reddit r/LocalLLaMA/r/privacy, and arXiv evals). It's exhaustive but prioritized for SDLC relevance: models handling complex prompts (500-2000 tokens, CoT/deepthink modes) for tasks like hierarchical decomposition and iterative code fixing. Exclusions: ChatGPT/Grok/Claude (limits), Perplexity.ai (soft caps), QuillBot (limitations noted in docs).

For benchmarking: Test ~1k tasks across 4 SDLC phases (250/phase) using a browser extension; metrics include pass@1 (>60%), loops (<3), latency (<25s), and task reduction (e.g., >20% fewer fixes). Start with a balanced model as baseline.

## Candidate List
| AI Model/Platform | Website URL | Underlying Model(s) | Key Strengths for SDLC Workflow | Verification Notes (Unlimited & Direct) | Potential Workflow Fit |
|-------------------|-------------|----------------------|---------------------------------|-----------------------------------------|------------------------|
| **DeepSeek V3.1** | [chat.deepseek.com](https://chat.deepseek.com) | DeepSeek-V3 (600B MoE) | Code gen (49.2% LiveCodeBench), reasoning (59.4% AIME), planning; low hallucination for research/fixing. | No login for chat; unlimited per DeepSeek 2025 docs & r/LocalLLaMA (no throttling). | Research/planning (80% reasoning tasks); fallback for complex logic. |
| **Qwen 3** | [chat.qwen.ai](https://chat.qwen.ai) | Qwen3 (72B, MoE like Qwen3-30B-A3B) | Code efficiency (65.8% SWE-Bench); fewer fixes (20-50% loops reduction in execution). | Alibaba free web; no caps per Qwen3 notes (arXiv 2508.09101) & Medium evals. | Execution (100% allocation to cut tasks); test for validation. |
| **GLM-4.6** | [chat.z.ai](https://chat.z.ai) | GLM-4.6 (400B MoE, 40B active) | Balanced agentic (81.2% MMLU-Pro, 33.8% SWE-Bench); fast hybrid CoT (5-25s) for all phases. | Zhipu web unrestricted (2025 roadmap, Eval.16x.engineer); no login for core. | 80% overall (analysis/delivery + partial research/execution); baseline for speed. |
| **Llama 3.1** | [huggingface.co/chat](https://huggingface.co/chat) | Meta-Llama-3.1 (8B-405B) | Versatile planning/code (80.6% MMLU-Pro); open-source for custom prompts. | HF Spaces public unlimited (HF docs); direct web, no auth. | Analysis/research (70% tasks); modular for variants. |
| **Mistral Nemo** | [chat.mistral.ai](https://chat.mistral.ai) | Mistral-Nemo (12B) | Logic mapping (68.7% Tau-Bench); efficient for research. | Mistral free tier no limits (arXiv 2503.05248 updates); direct chat. | Research (50% tasks); quick for validation. |
| **EaseMate AI ChatGPT Free** | [www.easemate.ai/chatgpt-free](https://www.easemate.ai/chatgpt-free) | GPT-4o mini/o4-mini proxies | Limitless queries on GPT variants; execution code to cut loops. | No payment/enrollment; daily quota-free (site claims). | Execution (50% to validate efficiency); test for robustness. |
| **Unlimited AI Chat** | [app.unlimitedai.chat](https://app.unlimitedai.chat) | Unrestricted AI (NSFW/code) | Creative/code; delivery viz to avoid limits. | No login/restrictions (2025 launch). | Delivery (30% for unrestricted). |
| **HotBot Free ChatGPT** | [www.hotbot.com/free-chatgpt](https://www.hotbot.com/free-chatgpt) | OpenAI API proxy | Unrestricted GPT; execution fixing. | No registration/limits (site). | Execution (40% to test reduction). |
