Saathi Ai - Mental Health Chatbot (Gen AI Powered)

A compassionate mental health support chatbot built using LangChain, Groq LLaMA-3.3, and ChromaDB, designed to provide thoughtful and empathetic responses to user queries.
🚀 Features

    Uses LLaMA-3.3-70B via Groq for ultra-fast, high-quality generation

    Semantic search over mental health documents using ChromaDB + HuggingFace Sentence Transformers

    Custom prompt engineering for empathetic and human-like responses

    PDF document ingestion and retrieval for contextual awareness

🛠️ Tech Stack

    LangChain

    Groq API (LLaMA-3.3-70B)

    HuggingFace (all-MiniLM-L6-v2)

    ChromaDB

    PyPDFLoader

    Google Colab / Jupyter

📁 Project Structure

Mental_Health_Chatbot_GEN_AI.ipynb
/data/                  # Folder containing mental health PDFs
/chroma_db/             # Persisted vector database

🧩 How It Works

    PDFs are loaded using DirectoryLoader and PyPDFLoader.

    Text is split into chunks using RecursiveCharacterTextSplitter.

    Embeddings are generated using sentence-transformers/all-MiniLM-L6-v2.

    A vector store is created with ChromaDB.

    A RetrievalQA chain is set up with custom prompts to encourage compassionate responses.

💻 Setup Instructions

    Install dependencies

pip install langchain_groq langchain_core langchain_community
pip install pypdf chromadb sentence_transformers

    Prepare your data

Place relevant mental health PDFs in the data/ folder.

    Set up environment variables

Set your Groq API Key in the notebook/code:

groq_api_key = "your_api_key_here"

    Run the Notebook

Launch the notebook and run all cells sequentially. The chatbot will initialize, process documents, and allow you to ask questions.
🤖 Sample Prompt

User: I'm feeling very anxious and overwhelmed.
Chatbot: I’m sorry you’re feeling this way. You're not alone...

📌 Notes

    This tool is not a replacement for professional mental health care.

    It can be used for awareness, education, or conversational simulations.

📈 Future Improvements

    Add UI using Streamlit or Gradio

    Integrate real-time chat interface

    Enhance context window and refine prompts
