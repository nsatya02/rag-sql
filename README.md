# rag-sql

how to create a custom agent that can query either your LlamaCloud index for RAG-based retrieval or a separate SQL query engine as a tool.

+----------------------------+
|      User                  |
|  - Uploads a PDF           |
|  - Asks queries            |
+------------+---------------+
             |  
             v
+-----------------------------+
|   RAG-SQL Agent              |
|  - Initializes models        |
|  - Creates SQL database      |
|  - Processes uploaded PDFs   |
|  - Creates AI agent          |
|  - Answers user queries      |
+-----------------------------+
