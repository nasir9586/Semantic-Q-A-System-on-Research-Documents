# 📘 Semantic Q&A System on Research Documents  
*A lightweight RAG-based pipeline using TinyLLaMA + Ollama + LangChain for research paper understanding.*

---

## 🚀 Project Overview

This project implements a **Semantic Question-Answering System** over research PDFs using Retrieval-Augmented Generation (RAG). It leverages:

- 📄 PDF loading via `LangChain`
- 🔍 FAISS vector store for semantic retrieval
- 🤖 `TinyLLaMA` model served through `Ollama` for lightweight language inference
- 🧠 HuggingFace embeddings for meaningful chunk retrieval

It allows users to ask questions about a paper (e.g., "What optimization techniques are used?") and receive accurate, context-aware answers grounded in the document.

---

## 🎯 Aim

To design a local, efficient, and intelligent assistant capable of reading and answering questions on academic research papers using semantic search and generative AI.

---

## 🎯 Objectives

- Load and preprocess PDF research papers.
- Convert documents into vector representations using transformer-based embeddings.
- Store and retrieve relevant content using FAISS vector search.
- Use `TinyLLaMA` for generating responses based on retrieved chunks.
- Support contextual chat with memory using LangChain’s `ConversationalRetrievalChain`.

---

## 🛠️ Technologies & Libraries

| Component       | Tech Used                |
|----------------|--------------------------|
| Language Model  | TinyLLaMA (1.1B params) via Ollama |
| Vector Store    | FAISS                    |
| Embeddings      | HuggingFace Embeddings   |
| Text Chunking   | LangChain Splitter       |
| PDF Loader      | PyPDFLoader              |
| Conversational Chain | LangChain Q&A Chain  |

---

## ⚙️ Model Info

- **Model Name:** TinyLLaMA (1.1B Parameters)
- **Link:** [TinyLLaMA on Ollama](https://ollama.com/library/tinyllama)
- **LLM Hosting:** Locally via [Ollama](https://ollama.com/)
- **Serving Type:** Conversational with memory

---

## 💡 Project Insights

- Efficiently extracts and answers from research papers.
- Uses semantic chunking with overlapping windows to preserve context.
- Provides human-like Q&A experience in local environment.
- Ideal for students and researchers working offline with limited compute.

---

## 🔍 Sample Query

```python
query = "What are different Indexing Optimization methods used in this paper"
