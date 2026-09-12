# Generative AI Document Q&A

An AI-powered Retrieval-Augmented Generation (RAG) system for question answering over PDF documents using semantic search, Chroma vector storage, Hugging Face embeddings, and Ollama.

## Overview

This project allows users to ask questions about the content of a PDF document and receive context-aware answers.

The system loads the PDF, splits its content into smaller text chunks, generates semantic embeddings, and stores them in a Chroma vector database. When a user asks a question, the system retrieves the most relevant document sections and provides them as context to a locally hosted Llama 3.2 model through Ollama.

## How It Works

The application follows a Retrieval-Augmented Generation workflow:

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
Llama 3.2 via Ollama
↓
Generated Answer

## Technologies Used

- Python
- LangChain
- PyPDF
- RecursiveCharacterTextSplitter
- Hugging Face Embeddings
- Chroma
- Ollama
- Llama 3.2
- all-MiniLM-L6-v2

## Key Features

- Question answering over PDF documents
- PDF document loading and text processing
- Text chunking with overlapping chunks
- Semantic embeddings using Hugging Face
- Vector storage and similarity search using Chroma
- Locally hosted LLM inference using Ollama
- Context-based answer generation

## Project Structure

generative-ai-document-qa/
│
├── company.pdf
├── document_qa.ipynb
├── README.md
└── requirements.txt

## Sample Document

The repository includes `company.pdf`, a sample employee-policy document used to demonstrate the document question-answering workflow.

Example questions include:

- What are the standard working hours?
- How many sick leave days are available?
- How many casual leave days are provided?
- Is work from home allowed?

## Purpose

This project demonstrates the core concepts of Retrieval-Augmented Generation, including document processing, text chunking, semantic embeddings, vector similarity search, context retrieval, and locally hosted LLM-based response generation.
