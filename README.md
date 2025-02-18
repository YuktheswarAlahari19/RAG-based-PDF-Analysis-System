# RAG-based PDF Analysis System

## Project Overview
This project implements a Retrieval-Augmented Generation (RAG) system for analyzing PDF documents. It uses a locally hosted DeepSeek 1.5B language model for efficient text processing and Cassandra DB for vector storage and retrieval.

## Features
- PDF document analysis and information extraction
- Integration with locally hosted DeepSeek 1.5B LLM
- Vector storage and retrieval using Cassandra DB
- Conversational interface for document queries using LangChain

## Technologies Used
- Python
- LangChain
- DeepSeek LLM (1.5B model)
- Cassandra DB (DataStax Astra)
- Docker (for Ollama model hosting)

## Setup Instructions
1. Clone the repository
2. Install required Python packages: `pip install -r requirements.txt`
3. Set up DataStax Astra account and download the necessary connection bundle
4. Add the DataStax connection bundle to the project directory
5. Install Ollama locally or use Docker to run the DeepSeek 1.5B model
6. Configure environment variables for database connection


## Limitations
- The DeepSeek 1.5B model used is a coder model, which may not provide highly accurate results for general text analysis
- Performance may vary based on the available system resources, especially GPU memory
- Requires active internet connection for DataStax Astra DB operations

## Future Improvements
- Implement more accurate general-purpose language models
- Optimize for better performance on systems with limited GPU memory
- Enhance the query processing pipeline for more accurate information retrieval

