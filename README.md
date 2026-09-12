# Generative AI Document Q&A

An AI-powered Retrieval-Augmented Generation (RAG) system for intelligent question answering over PDF documents.

## 📌 Overview

This project allows users to ask questions about the content of a PDF document and receive context-aware answers. Instead of relying only on the language model's existing knowledge, the system retrieves relevant information from the uploaded document and uses that context to generate the response.

## 🔄 How It Works

The application follows a simple RAG pipeline:

PDF Document  
↓  
Document Loading  
↓  
Text Chunking  
↓  
Semantic Embeddings  
↓  
Chroma Vector Database  
↓  
Similarity Search  
↓  
Relevant Context  
↓  
Local LLM with Ollama  
↓  
Generated Answer

## 🛠️ Technologies Used

- Python
- LangChain
- PyPDFLoader
- RecursiveCharacterTextSplitter
- Hugging Face Embeddings
- Chroma
- Ollama
- Llama 3.2
- all-MiniLM-L6-v2

## ✨ Key Features

- Ask questions about PDF documents
- Split documents into searchable text chunks
- Generate semantic embeddings for document content
- Retrieve relevant document sections using similarity search
- Generate answers using a locally hosted LLM
- Keep document information as the context for answering questions

## 🚀 Project Workflow

1. Load the PDF document.
2. Split the document into smaller overlapping chunks.
3. Generate embeddings for the document chunks.
4. Store the embeddings in Chroma.
5. Search for chunks relevant to the user's question.
6. Pass the retrieved context to the local LLM.
7. Generate a context-aware answer.

## 📂 Project Structure

```text
generative-ai-document-qa/
│
├── document_qa.ipynb
└── README.md
