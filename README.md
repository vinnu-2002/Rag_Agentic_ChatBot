# Rag_Agentic_ChatBot
 Agentic RAG Chatbot using Model Context Protocol (MCP) – A multi-format document QA assistant built with Python, Streamlit, HuggingFace, FAISS, and an agent-based architecture. Upload PDFs, PPTs, DOCX, CSVs, or TXT files and ask questions using a Retrieval-Augmented Generation pipeline powered by open-source LLMs.

# 🤖 Agentic RAG Chatbot for Multi-Format Document QA

An agent-based Retrieval-Augmented Generation (RAG) chatbot that uses Model Context Protocol (MCP) to answer user questions from uploaded documents of various formats (PDF, PPTX, DOCX, CSV, TXT/Markdown).

---

## 🔧 Features

- ✅ Supports uploading documents in: PDF, PPTX, DOCX, CSV, TXT/MD
- 🧠 Agentic architecture with 3 core agents:
  - **IngestionAgent** – Extracts and parses document content
  - **RetrievalAgent** – Uses HuggingFace embeddings + FAISS for semantic search
  - **LLMResponseAgent** – Uses open-source LLMs to generate final answers
- 📬 Message-passing via custom MCP protocol
- 💬 Streamlit UI for uploading files, asking questions, and viewing sources

---

## 🏗️ Architecture

![Architecture Diagram](./architecture.png)  <!-- replace with your actual diagram -->

---

## 🛠️ Tech Stack

| Component         | Tool / Library                 |
|------------------|-------------------------------|
| UI               | Streamlit                     |
| Embeddings       | HuggingFace (all-MiniLM-L6-v2)|
| Vector Store     | FAISS                         |
| LLM              | Google Flan-T5 (transformers) |
| Parsing PDFs     | PyMuPDF (fitz)                |
| DOCX / PPTX / CSV| python-docx, python-pptx, pandas |
| Communication    | Custom Model Context Protocol (MCP) |

