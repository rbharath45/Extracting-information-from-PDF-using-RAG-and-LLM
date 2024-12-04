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
Setup Instructions
Clone the Repository

bash
Copy code
git clone <repository-url>
cd <repository-folder>
Install Dependencies

bash
Copy code
pip install google-generativeai cohere sentence-transformers chromadb
Set Up API Keys

Obtain an API key for Google Generative AI and Cohere Rerank API.
Set them as environment variables:
bash
Copy code
export API_KEY=<Your_Google_API_Key>
export COHERE_API_KEY=<Your_Cohere_API_Key>
Run the Code

bash
Copy code
python main.py
Usage
Upload a PDF file.
The system extracts content and stores it in chunks using a vector database.
Query the system using natural language questions.
Get responses with or without reranking for comparison.
Key Functions
Content Extraction: Breaks the PDF into titled sections.
Embedding and Storage: Creates vector embeddings for efficient search.
Query Answering:
Baseline retrieval of documents.
Reranked retrieval using Cohere.
Context-based response generation.
Performance Comparison: Compares results with and without reranking.
Examples
Query: "What is the capital of the United States?"

Baseline: "Washington, D.C. is the capital of the United States."
Reranked: "Washington, D.C. is the capital of the United States. It is a federal district."
Query: "Explain the transport of food and substances in plants."

Generates a detailed response using extracted context.
Future Enhancements
Support for multi-file PDF processing.
Advanced error handling for unsupported file types.
Fine-tuning the embedding and reranking models for domain-specific applications.
Integration with web or mobile interfaces for easier usage.
