# Retrieval-Augmented Generation (RAG) from Scratch

A basic Retrieval-Augmented Generation (RAG) pipeline built from scratch using LangChain, Sentence Transformers, and ChromaDB.

This implementation demonstrates how documents are converted into embeddings, stored in a vector database, and retrieved using semantic search.

---

## What I implemented

- Loaded multiple PDF documents
- Extracted text from PDFs
- Split documents into smaller chunks using RecursiveCharacterTextSplitter
- Generated dense vector embeddings using Sentence Transformers
- Stored embeddings in a persistent ChromaDB vector database
- Performed semantic similarity search using vector embeddings
- Built a custom RAG retriever class for document retrieval

---

## Tech Stack

- Python
- LangChain
- Sentence Transformers
- ChromaDB
- PyMuPDF
- PyPDF
- NumPy

---

## Embedding Model

**all-MiniLM-L6-v2**

A lightweight Sentence Transformer model used to convert document chunks and user queries into dense vector embeddings.

---

## Vector Database

**ChromaDB**

Used as a persistent vector store to save document embeddings and perform semantic similarity search.

---

## Workflow

PDF Documents
↓
Load Documents
↓
Text Chunking
↓
Generate Embeddings
↓
Store Embeddings in ChromaDB
↓
User Query
↓
Generate Query Embedding
↓
Semantic Search
↓
Retrieve Most Relevant Chunks

---

## What I Learned

- The complete ingestion pipeline for a RAG system
- Why large documents need to be split into chunks
- How embedding models convert text into vectors
- How vector databases perform semantic search
- The difference between keyword search and vector similarity search
- How document retrieval forms the foundation of Retrieval-Augmented Generation

---

## Next Steps

- Integrate an LLM to generate answers from the retrieved context
- Experiment with different embedding models
- Compare ChromaDB with FAISS
- Build a FastAPI or Streamlit interface for interactive querying