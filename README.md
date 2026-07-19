# 🤖 Agentic AI Research Paper Intelligence System

An intelligent research assistant powered by **Agentic AI** that enables users to search, analyze, summarize, compare, and extract insights from research papers using Large Language Models (LLMs), semantic search, and autonomous tool selection.

The system combines **Retrieval-Augmented Generation (RAG)**, **vector search**, **LLMs**, and **Agentic AI** to provide an interactive experience for exploring scientific literature.

---

## 🚀 Features

- 🔍 Semantic Research Paper Search using Sentence Transformers
- 📚 Fast Similarity Search with FAISS
- 📝 Automatic Research Paper Summarization using BART
- 🏷️ Keyword Extraction using KeyBERT
- 🧠 Named Entity Extraction using Gemini
- ⚖️ Compare Two Research Papers
- 🤖 Agentic AI that automatically selects the appropriate tool based on user queries
- 📄 Structured Responses generated using Llama 3.1 (Groq)
- 📊 Similarity Ranking of Research Papers
- 📝 Agent Interaction Logging

---

# 🏗️ System Architecture

```
                         User Query
                              │
                              ▼
                   Agentic AI (LangChain Agent)
                              │
        ┌─────────────────────┼─────────────────────┐
        │                     │                     │
        ▼                     ▼                     ▼
 Search Papers         Extract Keywords      Compare Papers
        │                     │                     │
        ▼                     ▼                     ▼
 SentenceTransformer     KeyBERT            Llama 3.1
        │
        ▼
    FAISS Vector Search
        │
        ▼
 Retrieve Top-K Papers
        │
        ▼
 BART Summarization
        │
        ▼
 Gemini Entity Extraction
        │
        ▼
 Final AI Generated Response
```

---

# 🛠️ Tech Stack

### Programming Language

- Python

### Machine Learning

- Sentence Transformers
- Hugging Face Transformers
- KeyBERT
- Scikit-Learn

### LLMs

- Groq
- Llama 3.1 8B Instant
- Google Gemini 2.5 Flash

### Agent Framework

- LangChain
- LangChain Groq

### Vector Database

- FAISS

### Dataset

- ML-ArXiv Papers Dataset

---

# 📂 Project Structure

```
AI-Research-Paper-Intelligence-System/
│
├── notebooks/
│   └── AI_Research_Paper_Intelligence_System.ipynb
│
├── paper_embeddings.npy
├── paper_faiss.index
├── agent_log.json
├── requirements.txt
├── README.md
└── .gitignore
```

---

# ⚙️ Workflow

### Step 1

Load the ML-ArXiv dataset.

### Step 2

Clean and preprocess research papers.

### Step 3

Generate embeddings using SentenceTransformer.

### Step 4

Store embeddings inside a FAISS vector index.

### Step 5

User submits a research query.

### Step 6

Agent decides which tool should be executed.

Possible tools include:

- Search Research Papers
- Summarize Papers
- Extract Keywords
- Compare Papers

### Step 7

Retrieve Top-K similar papers.

### Step 8

Generate summaries using Facebook BART.

### Step 9

Extract important keywords using KeyBERT.

### Step 10

Extract research entities using Gemini.

### Step 11

Generate the final response using Llama 3.1.

---

# 🤖 Agentic AI Tools

### 🔍 Search & Summarize

- Searches relevant papers
- Retrieves Top-K results
- Generates concise summaries

---

### 🏷️ Keyword Extraction

Extracts important keywords using KeyBERT.

---

### ⚖️ Compare Papers

Compares two research papers based on:

- Objective
- Methodology
- Contributions
- Advantages
- Limitations
- Applications

---

# 📊 Dataset

**ML-ArXiv Papers**

Contains thousands of machine learning research papers with:

- Title
- Abstract

The dataset is used to build semantic embeddings for efficient retrieval. :contentReference[oaicite:0]{index=0}

---

# 📦 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/AI-Research-Paper-Intelligence-System.git
```

Move into the project

```bash
cd AI-Research-Paper-Intelligence-System
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# 🔑 Environment Variables

Create a `.env` file.

```
GROQ_API=your_groq_api_key
GOOGLE_API_KEY=your_google_api_key
```

---

# ▶️ Run

Open the notebook

```
AI_Research_Paper_Intelligence_System.ipynb
```

Run all cells sequentially.

---


# 📈 Future Improvements

- Streamlit Web Application
- Multi-Agent Workflow using LangGraph
- PDF Upload Support
- Research Paper Recommendation Engine
- Citation Network Visualization
- Interactive Dashboard
- ArXiv API Integration
- Memory-enabled Conversational Research Assistant

---

