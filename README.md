# RAG-Powered-Q-A-System-for-Duolingo-English-Test-Documentation
This notebook implements a Retrieval-Augmented Generation (RAG) system designed to answer domain-specific questions using official Duolingo English Test (DET) documentation.

The system ingests PDF documents, converts them into semantic embeddings, stores them in a FAISS vector database, and retrieves the most relevant document chunks when a user submits a question. The final response is generated strictly from retrieved context to ensure factual grounding and reduce hallucination.

This project demonstrates a practical implementation of semantic search and retrieval-augmented generation using modern NLP tools.

System Architecture

The pipeline follows these steps:

1.Document Ingestion
Load DET PDF documentation into structured document objects.

2.Text Chunking
Split documents into overlapping chunks to improve semantic retrieval accuracy.

3.Embedding Generation
Convert text chunks into vector embeddings using Sentence-Transformers.

4.Vector Storage (FAISS)
Store embeddings in a FAISS index for efficient similarity search.

5.Retrieval
Retrieve the top-k most relevant chunks based on cosine similarity.

6.Answer Generation
Generate a grounded response based solely on retrieved context.

Link to Jupyter Notebook:https://colab.research.google.com/drive/1eG9llk_orSbuWz5XfNyeo4zE8ELdmxsj?usp=sharing
