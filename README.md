# rag-sql

A custom AI agent that can query either your LlamaCloud index for RAG-based retrieval or a separate SQL query engine as a tool.

## Features

- **Dual Knowledge Base**  
  🔢 SQL Database for numerical data (populations, states)  
  📄 RAG System for PDF document analysis.

- **Smart Query Routing**  
  Automatic detection of question type (numerical vs descriptive)
  

- **Streamlit Web Interface**  
  🖥️ Interactive chat interface  
  📤 PDF upload capability

- **Open Source Stack**  
  🦙 Ollama LLM integration  
  🤗 Hugging Face embeddings  
  ☁️ LlamaCloud indexing

## Installation

1. **Clone Repository**
```bash
git clone https://github.com/yourusername/city-info-assistant.git
cd city-info-assistant

# Tech Stack 🛠️
Python (Streamlit, SQLAlchemy)
LlamaIndex (RAG, LLM agent)
Ollama (for LLM-based responses)
SQLite (in-memory database)

## Workflow 

![image](https://github.com/user-attachments/assets/3ef25349-a42a-4f95-94ed-c5684eae4e27)

