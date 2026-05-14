# 🤖 Wuilt Knowledge Base RAG Chatbot

A fully local **Retrieval-Augmented Generation (RAG)** chatbot built on top of a structured Markdown knowledge base. Uses **LangChain**, **Ollama**, and **ChromaDB** to answer questions about your docs — with a clean **Gradio** chat interface and interactive **t-SNE vector visualizations**.

---

## 🧠 How It Works

1. Loads Markdown files from a structured `wuilt-kb/` knowledge base
2. Splits documents into chunks and embeds them using `nomic-embed-text` via Ollama
3. Stores embeddings in a persistent **Chroma** vector store
4. Uses `llama3.2` (via Ollama) to answer questions with full conversation memory
5. Launches a **Gradio** chat UI for interactive Q&A

---

## ✨ Features

- 📁 **Multi-folder knowledge base** — automatically tags chunks by document type
- 🔍 **Semantic search** via ChromaDB vector retrieval
- 🧩 **Conversation memory** — remembers chat history across turns
- 📊 **2D & 3D t-SNE visualizations** of the embedding space using Plotly
- 💬 **Gradio chat interface** — runs in browser, shareable via public link
- 🔒 **Fully local** — no OpenAI API key needed

---

## 🛠️ Tech Stack

| Component        | Tool                          |
|------------------|-------------------------------|
| LLM              | `llama3.2` via Ollama         |
| Embeddings       | `nomic-embed-text` via Ollama |
| Vector Store     | ChromaDB                      |
| RAG Framework    | LangChain                     |
| Chat UI          | Gradio                        |
| Visualization    | Plotly + scikit-lea
