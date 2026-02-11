# 🧠 RAG-1: Retrieval-Augmented Generation Chatbot

An end-to-end Retrieval-Augmented Generation (RAG) based AI chatbot that
leverages open-source LLMs and vector databases to provide context-aware
answers from multiple data sources.

------------------------------------------------------------------------

## 🚀 Project Overview

RAG-1 is a GenAI project that combines:

-   🔍 Document Retrieval (Vector Search)
-   🧠 Open-source Large Language Models (LLMs)
-   📚 Multi-source data ingestion
-   ⚡ FastAPI / Streamlit based interface
-   🗂️ FAISS Vector Store

The system retrieves relevant chunks from documents and augments the LLM
prompt with contextual information before generating responses.

------------------------------------------------------------------------

## 🏗️ Architecture

User Query\
↓\
Embedding Generation\
↓\
FAISS Vector Search\
↓\
Relevant Context Retrieved\
↓\
LLM (LLaMA2 / Open Source Model)\
↓\
Final Context-Aware Response

------------------------------------------------------------------------

## 🛠️ Tech Stack

-   Python 3.10+
-   LangChain
-   FAISS
-   HuggingFace Embeddings
-   Open-source LLM (LLaMA2 / Mistral etc.)
-   FastAPI / Streamlit
-   Uvicorn
-   dotenv

------------------------------------------------------------------------

## 📂 Project Structure

    RAG-1/
    │
    ├── app.py
    ├── requirements.txt
    ├── .env
    ├── data/
    ├── embeddings/
    ├── vectorstore/
    ├── utils/
    └── README.md

------------------------------------------------------------------------

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

``` bash
git clone https://github.com/abhikghosh2049/RAG-1.git
cd RAG-1
```

### 2️⃣ Create Virtual Environment

``` bash
python -m venv venv
venv\Scripts\activate  # Windows
```

### 3️⃣ Install Dependencies

``` bash
pip install -r requirements.txt
```

### 4️⃣ Add Environment Variables

Create a `.env` file:

    OPENAI_API_KEY=your_key_here
    GROQ_API_KEY=your_key_here

### 5️⃣ Run the Application

For FastAPI:

``` bash
uvicorn app:app --reload
```

OR for Streamlit:

``` bash
streamlit run app.py
```

------------------------------------------------------------------------

## ✨ Features

-   Multi-document ingestion
-   Chunking using RecursiveCharacterTextSplitter
-   FAISS similarity search
-   Open-source LLM integration
-   Context-aware responses
-   Scalable architecture

------------------------------------------------------------------------

## 📈 Future Improvements

-   Add memory support (conversation history)
-   Deploy on cloud (AWS / Render / Vercel)
-   Add authentication layer
-   Improve UI/UX
-   Add streaming responses

------------------------------------------------------------------------

## 🧑‍💻 Author

**Abhik Ghosh**\
AI/ML & Data Science Enthusiast\
GitHub: https://github.com/abhikghosh2049

------------------------------------------------------------------------

## 📜 License

This project is open-source and available under the MIT License.

------------------------------------------------------------------------

⭐ If you found this project helpful, consider giving it a star!
