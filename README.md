# 🔍 RAG Course - Building Agentic RAG with LlamaIndex

A hands-on course exploring **Retrieval-Augmented Generation (RAG)** concepts using [LlamaIndex](https://www.llamaindex.ai/) and OpenAI. This repository contains Jupyter notebooks that progressively build up from basic tool calling to advanced multi-document agents.

---

## 📚 Course Notebooks

| # | Notebook | Description |
|---|----------|-------------|
| 1 | [Tool Calling](Tool_calling.ipynb) | Learn how LLMs can call external functions using LlamaIndex's `FunctionTool`. Covers defining custom tools (`add`, `mystery`) and letting the LLM decide which tool to invoke based on natural language queries. |
| 2 | [Router Engine](Router_engine.ipynb) | Build a **Router Query Engine** that intelligently routes queries to either a **vector index** (for specific questions) or a **summary index** (for summarization) over the MetaGPT paper. |
| 3 | [Building a Multi-Document Agent](Building_Multidocument_Agent.ipynb) | Scale up to an agent that can reason over **3 research papers** (MetaGPT, LongLoRA, Self-RAG) simultaneously, with per-document vector and summary tools. |
| 4 | [Agent Reasoning Loop](Agent_Reasoning_loop.ipynb) | Dive into the **agent reasoning loop** using `FunctionCallingAgentWorker` and `AgentRunner` to understand how agents plan, execute, and iterate through multi-step reasoning. |

---

## 🛠️ Tech Stack

- **[LlamaIndex](https://www.llamaindex.ai/)** — Data framework for LLM applications
- **[OpenAI GPT-3.5 Turbo](https://platform.openai.com/)** — LLM for generation and tool calling
- **[OpenAI Embeddings](https://platform.openai.com/)** — `text-embedding-ada-002` for vector search
- **Python** — Jupyter Notebooks

---

## 📄 Research Papers Used

The course uses the following papers for building RAG pipelines:

1. **MetaGPT** — Multi-agent framework for software engineering
2. **LongLoRA** — Efficient fine-tuning for long-context LLMs
3. **Self-RAG** — Learning to retrieve, generate, and critique through self-reflection

---

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- OpenAI API Key

### Installation

```bash
pip install llama-index openai nest_asyncio
```

### Set up your API key

```python
import os
os.environ["OPENAI_API_KEY"] = "your-api-key-here"
```

### Run the notebooks

```bash
jupyter notebook
```

---

## 📂 Project Structure

```
RAG_course/
├── Tool_calling.ipynb                  # Lesson 1: Function tool calling
├── Router_engine.ipynb                 # Lesson 2: Router query engine
├── Building_Multidocument_Agent.ipynb  # Lesson 3: Multi-document agent
├── Agent_Reasoning_loop.ipynb          # Lesson 4: Agent reasoning loop
└── README.md                           # This file
```

---

## 📝 Key Concepts Covered

- ✅ **Tool Calling** — Letting LLMs invoke external functions
- ✅ **Query Routing** — Directing queries to the right index type
- ✅ **Vector Search** — Semantic search over document chunks
- ✅ **Summary Index** — Full document summarization
- ✅ **Multi-Document Agents** — Reasoning across multiple sources
- ✅ **Agent Reasoning Loop** — Step-by-step agent execution and planning

---

## 📜 License

This project is for educational purposes.

---

⭐ **If you find this helpful, give it a star!**
