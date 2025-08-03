# YouTube Chatbo using LangChain (RAG Pipeline)

This project allows you to ask questions about YouTube videos by using **LangChain**, **LLMs**, and a **Retrieval-Augmented Generation (RAG)** system.
It fetches the transcript of a video, indexes it using embeddings, and answers questions using a language model.

---

## Features

- 🔗 Loads YouTube transcripts using `YouTubeLoader`
- ✂️ Splits long transcripts into chunks
- 🧠 Converts chunks into vector embeddings
- 📦 Stores vectors in a vector store (e.g. FAISS or Chroma)
- 🔍 Retrieves relevant chunks using semantic search
- 🤖 Uses LLM (like OpenAI or HuggingFace) to answer user queries based on retrieved context

---

## Tech Stack

- [LangChain](https://www.langchain.com/)
- [YouTubeLoader](https://python.langchain.com/docs/modules/data_connection/document_loaders/integrations/youtube/)
- [FAISS](https://github.com/facebookresearch/faiss) / [Chroma](https://www.trychroma.com/)
- [OpenAI](https://openai.com/) / HuggingFace LLMs
- Python

---

## How It Works

1. **Input:** YouTube URL  
2. **Transcript Extraction:** Using `YouTubeLoader`  
3. **Chunking:** TextSplitter splits transcript into smaller pieces  
4. **Embedding:** Convert chunks into vector embeddings  
5. **Vector Store:** Save vectors to a store  
6. **Query:** User enters a question  
7. **Retriever:** Finds relevant transcript chunks  
8. **LLM:** Uses chunks + question to generate an answer

---
