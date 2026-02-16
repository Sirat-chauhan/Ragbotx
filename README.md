

# 🤖 RagBotX

### Advanced RAG Chatbot with GraphRAG & Persistent Chat Memory

**100% Local • Fully Private • Powered by Ollama**

RagBotX is a fully offline Retrieval-Augmented Generation (RAG) chatbot that lets you upload documents and ask intelligent, contextual questions — all without sending data to external APIs.

Built with Python, Streamlit, FAISS, LangChain, and Ollama.

---

## 🚀 Why RagBotX?

Most RAG systems stop at vector search.

RagBotX goes further:

* 🔎 Hybrid Retrieval (Vector + Reranking)
* 🌐 GraphRAG (Knowledge Graph–enhanced reasoning)
* 🧠 Chat Memory (Multi-turn awareness)
* 🎯 HyDE Query Expansion (Improved recall)
* 🔒 100% Offline & Private
* ⚡ Fast, lightweight, and configurable

Everything runs locally using Ollama.

---

# ✨ Features

## 📂 Document Upload

* Upload **PDF**, **DOCX**, or **TXT**
* Automatic chunking & indexing

## 🔎 Hybrid Retrieval Pipeline

* FAISS vector search
* Neural reranking
* Improved semantic precision

## 🌐 GraphRAG

* Builds a lightweight Knowledge Graph
* Expands context using graph relationships
* Enhances deep document understanding

## 🧠 Persistent Chat Memory

* Remembers previous conversation turns
* Maintains contextual continuity

## 🎯 HyDE Query Expansion

* Generates hypothetical answers
* Uses them to improve document retrieval quality

## 🔄 Dual Mode Operation

* **RAG Mode** → Context-aware document Q&A
* **Chat Mode** → General AI conversation

## 🎛️ Fully Customizable

* Model selection
* Temperature control
* Max retrieved contexts
* Toggle HyDE / Reranking / GraphRAG

---

# 🖥️ How It Works

```
User Query
   ↓
HyDE Expansion (optional)
   ↓
FAISS Retrieval
   ↓
Neural Reranking (optional)
   ↓
GraphRAG Context Expansion (optional)
   ↓
Chat Memory Injection
   ↓
Ollama LLM Response
```

All computation happens locally.

No cloud. No tracking. No API keys.

---

# 📦 Installation

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/siratchauhan/RagBotX.git
cd RagBotX
```

## 2️⃣ Create Virtual Environment

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### Mac/Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

## 3️⃣ Install Dependencies

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

---

## 4️⃣ Install Ollama & Pull Models

Download Ollama:
[https://ollama.ai](https://ollama.ai)

Then pull required models:

```bash
ollama pull qwen2:0.5b
ollama pull nomic-embed-text
```

You can change models later in the `.env` file.

---

## 5️⃣ Configure Environment

Create a `.env` file in the project root:

```
DEFAULT_MODEL=qwen2:0.5b
EMBEDDINGS_MODEL=nomic-embed-text
ENABLE_HYDE=true
ENABLE_RERANKING=true
ENABLE_GRAPH_RAG=true
TEMPERATURE=0.7
MAX_CONTEXTS=3
```

---

## 6️⃣ Start Ollama

```bash
ollama serve
```

---

## 7️⃣ Launch RagBotX

```bash
streamlit run app.py
```

---

# 🧪 Use Cases

* 📚 Research assistant
* 📄 Legal / contract analysis
* 🏢 Private company knowledge base
* 🎓 Study companion
* 🔐 Air-gapped environments

---

# 🛣️ Roadmap

* Suggested follow-up questions
* Graph visualization UI
* Export Knowledge Graph as JSON
* Support for alternative vector databases
* Advanced RAG pipelines (Basic vs Graph-Enhanced)
* Multi-document collection management

---

# 🧠 Tech Stack

* Python
* Streamlit
* FAISS
* LangChain
* Ollama

---

# 🤝 Contributing

Pull requests, ideas, and feedback are welcome!

If you find this project useful, consider giving it a ⭐

