# Hybrid RAG & SQL Query Engine🚀

The intelligent query capabilities of your system, seamlessly integrating retrieval-augmented generation (RAG) and Text-to-SQL into a single AI-powered interface.

A hybrid AI assistant combining SQL data analysis and RAG document retrieval to answer for user queries. Built with a modern tech stack, it intelligently routes queries to the appropriate tool (SQL or RAG or both) for accurate and context-aware responses.

# Index creation(Manually & API)📖🔄
- **USE app.py :**
  If you are able to create an index using API then use "app.py". In the code there are all the configurations like which vector database(by default llama),
  embedding model and chunking strategy should be used. You can modify them as per your requirements.
  
  If it is working for you just run "app.py" automatically the index will be created in llamacloud--> index.
  
  It worked for me fine for some period of time but later for some unknown reasons i'm unable to create an index using API. 


- **USE app1.py :**
  If you are unable to create index using API. By following the below steps you can create it manually :
  1. Open llamacloud.
  2. Go to indexes.
  3. Click create index.
  4. upload your documents.
  5. select/create your vector Database(by default managed by llamacloud).
  6. select/create your embedding model.(In this Huggingface embeddings is used).
  7. Transform settings----> choouse your chunking strategy(Auto/Manual).
  8. click deploy index.

**Then copy the index endpoint details and use them in the code.**

## Installation and setup⚙️

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

## Workflow📊

![image](https://github.com/user-attachments/assets/3ef25349-a42a-4f95-94ed-c5684eae4e27)



