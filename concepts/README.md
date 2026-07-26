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

### [Embeddings & Vector Search](embeddings/)

Turning text into numbers so machines can find "similar" meaning.

| Page | What it covers |
|---|---|
| [Embeddings & Vector Search](embeddings/README.md) | What a vector is, the embedding space, cosine vs dot product vs Euclidean, exact k-NN vs HNSW, failure modes, picking a model |

---

## 🚧 Planned

| Concept | In one line |
|---|---|
| Chunking Strategies | How you split documents — and why it makes or breaks retrieval |
| Prompt Engineering | Structuring what you send the model to get what you want back |
| Fine-tuning vs RAG | Two ways to specialize a model, and when to reach for each |
| AI Agents & Tool Use | Letting a model take actions, not just answer |
| Model Context Protocol (MCP) | A standard way to plug tools and data into models |
| Evaluating AI Systems | How you actually measure whether any of this works |

---

← Back to [home](../README.md)
