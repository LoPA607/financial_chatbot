# financial_chatbot
# 🧠 Chatbot using LLaMA-2, LangChain & Streamlit

This project is an interactive chatbot built with **Streamlit**, powered by **LLaMA-2** and **LangChain**. It allows users to ask questions based on the content of local PDF documents and get intelligent responses using retrieval-augmented generation (RAG).

> ⚡ Ask anything related to the content in your PDF files. Useful for personal assistants, document Q&A, or domain-specific bots (e.g., health, law, research).

---

## Features

- 📁 Loads and processes all PDFs in the `data/` directory.
- 🧩 Splits text into manageable chunks using recursive splitting.
- 🤗 Uses `sentence-transformers/all-MiniLM-L6-v2` for semantic search.
- 🔎 FAISS vector store for fast document retrieval.
- 🧠 LLaMA-2 7B chatbot via `CTransformers` (quantized `.ggmlv3` model).
- 💬 Conversational memory with contextual replies.
- 🌐 Streamlit-based UI with persistent chat history.

---

## Requirements

Install dependencies via:

```bash
pip install -r requirements.txt

## Folder Structure
.
├── app.py              # Main Streamlit app
├── data/               # Folder to store all your PDF documents
├── models/             # (Optional) Folder to store .bin model files like llama-2-7b
└── README.md

## Run the app
streamlit run app.py
