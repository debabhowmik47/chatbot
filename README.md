This project loads a PDF → splits it into clean overlapping chunks → generates embeddings → stores them in ChromaDB → retrieves the most relevant text → and uses a local LLM to produce accurate answers grounded only in the PDF.

✔ Works 100% offline
✔ Runs a 7B parameter LLM locally
✔ Fast and accurate retrieval using ChromaDB
✔ Uses high-quality BGE embeddings
✔ Fully customizable RAG pipeline
✔ Ideal for budgets, research papers, legal PDFs, textbooks, etc.

RAG Architecture
PDF → Chunking → Embeddings → ChromaDB → Query → Retrieval → LLM → Answer

 Tech Stack
| Component        | Technology                         |
| ---------------- | ---------------------------------- |
| PDF Loader       | LangChain PyPDFLoader              |
| Text Splitter    | LangChain CharacterTextSplitter    |
| Embedding Model  | BAAI/bge-base-en-v1.5              |
| Vector DB        | ChromaDB                           |
| Local LLM        | Mistral-7B OpenOrca (GGUF)         |
| Inference Engine | llama-cpp-python                   |
| Platform         | Python 3.x / Google Colab          |
| Additional       | HuggingFace Hub for model download |
