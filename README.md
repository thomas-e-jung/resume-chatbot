## There is a known [GitHub issue](https://github.com/orgs/community/discussions/155944) where Jupyter notebooks fail to render in the browser from time to time. If this happens, please [open in Colab](https://colab.research.google.com/github/thomas-e-jung/resume-chatbot/blob/main/resume_chatbot.ipynb).

# Resume Chatbot

Author: Thomas Jung

## Overview
Resume Chatbot is a Python-based implementation of **Retrieval-Augmented Generation (RAG)** designed to utilize PDF documents, like resumes, as contextual data for generating responses to user queries.

## Features
- **PDF Input Files**: Parses user input files in PDF format for relevant context.
- **RAG Methodology**: Combines retrieval techniques with generative AI for accurate responses.
- **Customizable LLMs**: Uses HuggingFace embeddings and pipelines for text processing and generation.
- **Optimization**: Utilizes GPUs and 4-bit quantization for enhanced performance.

## Components
- **Embeddings Model**: [thenlper/gte-small](https://huggingface.co/thenlper/gte-small)
- **Chat Model**: [HuggingFaceH4/zephyr-7b-beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta)
- **Vector Store**: [Faiss](https://github.com/facebookresearch/faiss)

## Dependencies
To run in Google Colab, ensure the following packages are installed:
```bash
%pip install -U -q langchain_community pypdf bitsandbytes faiss-cpu
```
Additionally, ensure GPU runtime is enabled: Runtime tab > Change runtime type > T4 GPU.
