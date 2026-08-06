# AI Engineer Interview Preparation — Learn With Me 🚀

Hi, I'm Heer! I'm preparing for AI Engineering interviews, and instead of studying alone, I'm doing it in public — one module at a time. This repo is my living study guide: every module I work through gets polished into a visual, interview-focused reference and published here so you can **learn along with me**.

If you're on the same journey, star ⭐ the repo and follow along — new modules land as I complete them.

**🌐 Read everything on the site: [heeerrhkapadia.github.io/ai-engineer-interview-preparation](https://heeerrhkapadia.github.io/ai-engineer-interview-preparation/)**

## How to use this repo

Each module is a self-contained HTML study guide — richly formatted with diagrams, interview-style Q&A framing, callouts for pitfalls, and content kept current with the latest techniques.

**To read a module:**
1. Browse the [site](https://heeerrhkapadia.github.io/ai-engineer-interview-preparation/) — every module gets its own page, e.g. [📖 Module 1 — LLM Fundamentals](https://heeerrhkapadia.github.io/ai-engineer-interview-preparation/modules/module-01-llm-fundamentals.html), **or**
2. Download the `.html` file from the [`modules/`](modules/) folder and open it in any browser.

## Modules

| # | Module | Status |
|---|--------|--------|
| 01 | [LLM Fundamentals](https://heeerrhkapadia.github.io/ai-engineer-interview-preparation/modules/module-01-llm-fundamentals.html) | ✅ Available |
| 02 | [Prompt Engineering](https://heeerrhkapadia.github.io/ai-engineer-interview-preparation/modules/module-02-prompt-engineering.html) | ✅ Available |
| 03–12 | More modules on the way — agents, RAG, evals, fine-tuning, serving & more | 🔜 In progress |

## What's inside Module 1 — LLM Fundamentals

A ground-up tour of how large language models actually work, framed the way interviewers ask about it:

- **A · Foundations** — foundation models, what an LLM is, inference inside ChatGPT, autoregressive generation, open vs. closed source
- **B · The Transformer** — architecture, encoder/decoder variants, residual connections + FFN
- **C · Tokens & Embeddings** — tokenization & BPE, embeddings, positional encoding & RoPE
- **D · Attention** — Q/K/V self-attention, √dₖ scaling & softmax, causal masking, multi-head → GQA → MLA, Flash Attention, KV cache
- **E · Normalization** — LayerNorm & RMSNorm
- **F · Generation** — logits, context windows, temperature, top-k/top-p sampling, first-token latency, cross-entropy loss
- **G · Scaling & Efficiency** — Mixture of Experts, distillation, SLMs & LRMs
- **H · Alignment** — RLHF, PPO, DPO, GRPO
- **I · Frontier** — RLMs, DLMs, continual learning, ViT
- **J · Production** — troubleshooting drills for real-world scenarios

## What's inside Module 2 — Prompt Engineering

How to get reliable, structured, safe behaviour out of a model — and what goes wrong when you don't:

- **A · Foundations** — what prompt engineering is and why it matters, prompt anatomy & templates, system prompts & roles, prompt engineering vs. prompt tuning
- **B · Shot-based prompting** — zero-shot, one-shot, few-shot
- **C · Reasoning** — Chain-of-Thought, self-consistency, Tree-of-Thoughts, ReAct
- **D · Composition** — prompt chaining, meta-prompts & DSPy
- **E · Structured Output** — JSON/XML output and parsers
- **F · Context** — multi-turn conversations, "lost in the middle," multilingual prompting
- **G · Security** — prompt injection, jailbreaking
- **H · Optimize & Evaluate** — cost & latency, evaluating and iterating on prompts, common failure modes
- **J · Production** — troubleshooting drills for real-world scenarios

## Why "learn with me"?

Teaching is the best way to learn. By turning my prep notes into something worth sharing, I force myself to actually understand each concept well enough to explain it — and hopefully save you some of the hours I spent piecing this together.

Found a mistake or have a suggestion? Open an issue — I'd love the feedback.

## How the site is published

Every module lives on `main`. A workflow ([`deploy-pages.yml`](.github/workflows/deploy-pages.yml))
force-syncs `main` onto the `gh-pages` branch, and GitHub Pages serves that branch verbatim
(`.nojekyll` skips the Jekyll build). So a page on `main` becomes live once the sync runs *and*
Pages rebuilds.

If a module 404s on the site even though the file is in [`modules/`](modules/), the Pages build is
behind — check the **Actions** tab for a queued or failed *Publish to GitHub Pages* / *pages build
and deployment* run. Until it catches up, download the `.html` from `modules/` and open it locally.

The `main` → `gh-pages` hop is only there because Pages was pointed at `gh-pages`. Pointing
**Settings → Pages → Source → Deploy from a branch → `main` / (root)** would remove the workflow
from the critical path entirely — merges to `main` would publish directly.

## License

Released under the [MIT License](LICENSE). Learn freely, share freely.
