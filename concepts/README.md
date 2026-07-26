# Concepts

Every concept lives in its own folder. Each folder follows the same shape:

```
concepts/<concept>/
├── README.md          # the concept explained, diagrams first
├── <deep-dive>.md     # optional longer write-ups on sub-topics
└── diagrams/          # every .svg used on the pages above
```

---

## ✅ Live

### [Retrieval-Augmented Generation (RAG)](rag/)

How an LLM answers questions using *your* data instead of guessing.

| Page | What it covers |
|---|---|
| [RAG, from zero](rag/README.md) | The data flow, the indexing and retrieval pipelines, glossary |
| [Contextual Retrieval](rag/contextual-retrieval.md) | Why chunking destroys context, contextual embeddings + BM25, reranking, vector DBs, chunk sizing |

---

## 🚧 Planned

| Concept | In one line |
|---|---|
| Embeddings & Vector Search | Turning text into numbers so machines can find "similar" meaning |
| Chunking Strategies | How you split documents — and why it makes or breaks retrieval |
| Prompt Engineering | Structuring what you send the model to get what you want back |
| Fine-tuning vs RAG | Two ways to specialize a model, and when to reach for each |
| AI Agents & Tool Use | Letting a model take actions, not just answer |
| Model Context Protocol (MCP) | A standard way to plug tools and data into models |
| Evaluating AI Systems | How you actually measure whether any of this works |

---

← Back to [home](../README.md)
