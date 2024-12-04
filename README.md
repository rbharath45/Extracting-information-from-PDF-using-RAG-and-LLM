AI-Driven Contextual Information Extraction and Query Response System

This project demonstrates an end-to-end pipeline for extracting, processing, and querying information from PDF documents using advanced AI models and vector databases. The system combines generative AI, embeddings, and reranking techniques to deliver accurate and contextually relevant answers to user queries.

Features
PDF Content Extraction: Extracts and structures content into titled sections.
Embedding Generation: Converts text chunks into vector representations using a pre-trained model.
Vector Database Management: Stores and queries embeddings for efficient document retrieval.
Reranking: Uses a Cohere model to rank documents based on relevance to a user query.
Generative Responses: Leverages Google Generative AI to provide detailed answers based on context.
Technologies Used
Google Generative AI: For text extraction and answer generation.
Cohere Rerank API: For improving the relevance of retrieved documents.
SentenceTransformers: To generate embeddings for text chunks.
ChromaDB: For persistent vector storage and querying.
Python: The main programming language.

Dependencies:
google-generativeai
cohere
sentence-transformers
chromadb

Future Enhancements
Support for multi-file PDF processing.
Advanced error handling for unsupported file types.
Fine-tuning the embedding and reranking models for domain-specific applications.
Integration with web or mobile interfaces for easier usage.
