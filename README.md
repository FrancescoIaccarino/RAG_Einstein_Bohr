# 🧠 Beyond the Pages: Bringing Einstein and Bohr to Life with Retrieval-Augmented Generation

This project simulates historically faithful scientific personas — Albert Einstein and Niels Bohr — using Retrieval-Augmented Generation (RAG). By combining semantic search with neural text generation, we enable dynamic conversations grounded in authentic writings.

## 📚 Overview

- 🧲 **Retrieval**: Uses Sentence-BERT to identify relevant content from corpora of Einstein’s and Bohr’s letters, papers, and public writings.
- 🧠 **Generation**: A GPT-Neo model generates first-person responses in the style of each scientist.
- 🧬 **Personalization**: Each persona is grounded in a separate corpus, preserving tone, philosophy, and rhetorical quirks.

> “Imagine Newton debating Darwin. Curie explaining radiation to Feynman. This is just the beginning.”

## 🔧 Tech Stack

- 🧠 `GPT-Neo 1.3B` for response generation  
- 🔍 `Sentence-BERT (MiniLM-L6-v2)` for semantic retrieval  
- 📚 `FAISS` for efficient dense vector indexing  
- 🧼 Corpus preprocessing with Python (regex, filtering, chunking)  
- 📊 Evaluation with custom metrics: `StyleSim`, `QuerySim`, `Repetition Score`

## 📈 Results

- ✅ Best performing model: GPT-Neo 1.3B with high stylistic fidelity
- 🎯 Evaluation Metrics:
  - StyleSim: stylistic alignment with source persona
  - QuerySim: semantic relevance to user input
  - Repetition: lexical variety in generation

See slides/report for detailed visualizations and metrics.

## 🧪 What We Learned

- Dynamic persona modeling is viable without fine-tuning
- RAG is powerful for grounding LLMs in style-specific context
- Historical scientists can be brought into modern debates with AI

## 🛣️ Next Steps

- Expand to other personas (Marie Curie, Newton, Darwin)
- Add multi-turn dialogue flow
- Train custom embeddings for stylistic vectors


---

> "At any rate, I am convinced that He [God] does not throw dice."  
> — Albert Einstein

> "Einstein, stop telling God what to do."  
> — Niels Bohr
