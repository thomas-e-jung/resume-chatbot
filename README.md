# Resume Chatbot

Author: [Thomas Jung](mailto:thomas.e.jung@gmail.com)

## Overview
Resume Chatbot is a Python-based implementation of **Retrieval-Augmented Generation (RAG)** designed to utilize PDF documents, like resumes, as contextual data for generating responses to user queries.

## Features
- **PDF Input Files**: Parses user input files in PDF format for relevant context.
- **RAG Methodology**: Combines retrieval techniques with generative AI for accurate responses.
- **Customizable LLMs**: Uses HuggingFace embeddings and pipelines for text processing and generation.
- **Optimization**: Utilizes GPUs and 4-bit quantization for enhanced performance.

## Dependencies
To run in Google Colab, ensure the following libraries are installed:
```bash
%pip install -U -q langchain_community pypdf bitsandbytes faiss-cpu
```
Additionally, ensure GPU runtime is enabled: Runtime tab > Change runtime type > T4 GPU
