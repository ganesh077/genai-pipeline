# GenAI Pipeline with Retrieval-Augmented Generation (RAG)

This repository contains a Langflow-based GenAI pipeline that leverages vector embeddings and AstraDB to build a Retrieval-Augmented Generation (RAG) application. The pipeline ingests unstructured data, processes and embeds the text using a transformer model, stores the embeddings in AstraDB, and retrieves the most relevant context for generating answers with a language model.

## Features

- **Data Ingestion:**  
  Load and parse unstructured data (CSV, PDF, etc.) using custom Python scripts and Langflow components.

- **Text Processing & Splitting:**  
  Split long text documents into manageable chunks using a dedicated Split Text component.

- **Embedding Generation:**  
  Generate vector embeddings using transformer-based models (e.g., Hugging Face’s `sentence-transformers/all-MiniLM-L6-v2`).

- **Vector Storage in AstraDB:**  
  Store embeddings along with metadata in AstraDB using a custom schema with vector support.

- **Retrieval-Augmented Generation (RAG):**  
  Retrieve contextually relevant documents based on a user query’s embedding and combine them with the query to generate an answer with an LLM.

- **Modular & Scalable Architecture:**  
  The pipeline is built using Langflow’s visual interface and configuration JSON, making it easy to modify and extend.

## Repository Structure


https://github.com/user-attachments/assets/006e70d9-da7a-4d80-bdc6-87a3fd27bf83

