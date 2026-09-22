# PDF RAG Chatbot

A Retrieval-Augmented Generation (RAG) pipeline that lets you ask questions about any PDF document and get accurate, context-grounded answers.

## How it works
1. Load a PDF and split it into text chunks
2. Convert chunks into embeddings using Sentence Transformers
3. Store embeddings in a FAISS vector database for fast similarity search
4. On each question, retrieve the most relevant chunks and pass them to an LLM (Groq's GPT-OSS model) to generate an answer grounded in the document

## Tech stack
- Python
- LangChain
- FAISS (vector store)
- Sentence Transformers (embeddings)
- Groq API (LLM inference)

## Example
**Q:** What is this document about?
**A:** The document is a résumé (CV) summarizing background, professional experience, and technical skills.

## Run it yourself
Open the notebook in Google Colab, install the requirements in the first cell, upload a PDF, and add your own Groq API key.
