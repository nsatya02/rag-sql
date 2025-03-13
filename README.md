# Hybrid RAG & SQL Query Engine

The intelligent query capabilities of your system, seamlessly integrating retrieval-augmented generation (RAG) and Text-to-SQL into a single AI-powered interface.

A hybrid AI assistant combining SQL data analysis and RAG document retrieval to answer for user queries. Built with a modern tech stack, it intelligently routes queries to the appropriate tool (SQL or RAG) for accurate and context-aware responses.

## Installation

1. **Clone Repository**
```bash
git clone https://github.com/nsatya02/rag-sql.git
cd rag-sql
```
2. **Install Dependencies**
```bash
pip install -r requirements.txt
```
3. **Set Up Ollama**
```bash
ollama pull <eg:llama3.2>
```
4. **Configure Environment**
Create a .env file:
```bash
LLAMA_CLOUD_API_KEY=your_llama_cloud_key
HF_TOKEN=your_huggingface_token
```
5. **Run the Application**
```bash
streamlit run app.py(use when creating index using api) or app1.py(use when creating index manually)
```

## Features🚀

- **Dual Knowledge Base**  
  🔢 SQL Database for numerical data (populations, states)  
  📄 RAG System for PDF document analysis.

- **Smart Query Routing**  
  Automatic detection of question type (numerical vs descriptive)

- **Tech Stack 🛠️**
  Python (Streamlit, SQLAlchemy)
  LlamaIndex (RAG, LLM agent)
  Ollama (for LLM-based responses)
  SQLite (in-memory database)

- **Streamlit Web Interface**  
  🖥️ Interactive chat interface  
  📤 PDF upload capability

- **Open Source Stack**  
  🦙 Ollama LLM integration  
  🤗 Hugging Face embeddings  
  ☁️ LlamaCloud indexing

## Workflow 

![image](https://github.com/user-attachments/assets/3ef25349-a42a-4f95-94ed-c5684eae4e27)



