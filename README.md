<div align="center">

# 📚 Chat with Multiple PDFs
**An intelligent Conversational AI Agent for your Documents**

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://streamlit.io/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)](#)
[![LangChain](https://img.shields.io/badge/LangChain-Integration-green?logo=chainlink)](#)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4o--mini-orange)](#)

</div>

---

## ✨ Overview

*Chat with Multiple PDFs* is an interactive web application built with Streamlit and LangChain that allows you to upload multiple PDF documents and converse with them. It reads the text, processes it into semantic chunks, and sets up a conversational interface where you can ask questions and receive answers contextually sourced from your own documents.

## 🚀 Features

- **Multi-Document Support**: Upload multiple PDF files simultaneously.
- **Smart Retrieval**: Uses **OpenAI Embeddings (`text-embedding-3-small`)** and **FAISS** vector store for fast, accurate text retrieval.
- **Conversational Memory**: Retains the context of your chat history, allowing for natural, flowing conversations.
- **Powered by GPT-4o-mini**: Delivers fast and intelligent responses grounded in the uploaded context.
- **Sleek UI**: Built entirely in Streamlit with custom CSS.

## 🏗️ How it Works

1. **Document Loading**: PyPDF2 extracts text from uploaded PDFs.
2. **Text Splitting**: The text is chunked into manageable semantic pieces.
3. **Embeddings & Vector Store**: Text chunks are embedded using OpenAI Embeddings and stored locally via FAISS.
4. **Chat Interface**: A Conversational Retrieval Chain processes user queries against the vector store and generates answers using GPT-4o-mini!

<div align="center">
  <img src="./System Plan.png" alt="System Architecture" width="80%">
</div>

## 🛠️ Installation & Setup

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/Chat-with-Multiple-PDFs.git
cd "Chat with Multiple PDFs"
```

### 2. Set up the Python virtual environment

For Windows:
```bash
python -m venv .chatPdf
.chatPdf\Scripts\activate
```

For macOS/Linux:
```bash
python3 -m venv .chatPdf
source .chatPdf/bin/activate
```

### 3. Install Dependencies

Using `pip`:
```bash
pip install streamlit pypdf2 langchain python-dotenv faiss-cpu openai huggingface_hub langchain_openai langchain_community
```

### 4. Set Environment Variables

Create a `.env` file in the root directory and add your API keys:

```env
OPENAI_API_KEY=your_openai_api_key_here
```

## 🎮 Usage

Run the Streamlit application using the following command:

```bash
streamlit run app.py
```

- A browser window will automatically open `http://localhost:8501`.

<img width="1911" height="516" alt="Image" src="https://github.com/user-attachments/assets/71321f97-b2a2-4b2a-90ac-322255439e86" />

- Use the sidebar to **Upload your PDFs** and click **Process**.
- Start asking questions about your documents in the main chat input!

<img width="1912" height="1025" alt="Image" src="https://github.com/user-attachments/assets/a0f5e5a7-bb30-4ae1-8a50-c5653f6756ea" />

<img width="1918" height="1030" alt="Image" src="https://github.com/user-attachments/assets/e5104ca7-81ea-4baa-8a49-e3eafc488189" />

---
*Built with ❤️ using LangChain and Streamlit.*
