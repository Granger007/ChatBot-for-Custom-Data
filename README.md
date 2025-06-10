# 📄 Chatbot for Your Data

A simple, functional chatbot that allows users to interact with their own PDF documents using natural language. Built using **Flask**, **Langchain**, and **Retrieval-Augmented Generation (RAG)**, the chatbot extracts relevant information from the document and uses an LLM (like OpenAI's GPT) to answer user queries.

---

## 🚀 Features

* 🧠 Chat with any PDF file using LLMs (Large Language Models)
* 🔍 Retrieval-Augmented Generation (RAG) to provide accurate, context-aware answers
* 🌐 Web interface built with Flask
* 📚 Uses Langchain to manage document ingestion, chunking, embedding, and retrieval

---

## 💠 Tech Stack

* **Python**
* **Flask** – Web server and frontend interface
* **Langchain** – LLM framework for RAG pipelines
* **OpenAI API** – For language generation
* **FAISS / Chroma** – For vector-based document retrieval
* **PyMuPDF / pdfplumber** – For PDF parsing

---

## 📂 Project Structure

```
chatbot-for-your-data/
├── app.py                  # Flask backend
├── templates/
│   └── index.html          # Frontend UI
├── static/
│   └── styles.css          # Basic styling
├── utils/
│   └── rag_pipeline.py     # PDF loading, chunking, embedding, and querying
├── uploads/
│   └── (user PDFs)         # Uploaded PDF files
├── requirements.txt        # Python dependencies
└── README.md               # Brief Idea about the project
```

---

## ⚙️ Setup Instructions

1. **Clone the repo**

   ```bash
   git clone https://github.com/your-username/chatbot-for-your-data.git
   cd chatbot-for-your-data
   ```

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Set up your OpenAI API key**

   ```bash
   export OPENAI_API_KEY=your_openai_key_here
   ```

4. **Run the app**

   ```bash
   python app.py
   ```

5. **Open your browser** Go to `http://localhost:5000` to interact with the chatbot.

---

## 🧪 How It Works

* Upload a PDF file via the web interface.
* The system reads and splits the document into chunks.
* Embeddings are created and stored in a vector database.
* When a user types a question, relevant chunks are retrieved and passed to the LLM.
* The LLM generates a context-based answer using both the question and retrieved document chunks.

---

## 📌 To Do / Improvements

* Add multi-PDF support
* File caching for faster reloading
* Add file type support (e.g., DOCX)
* Integrate speech input and TTS output (future extension)
---

## 🙌 Acknowledgements

* [Langchain](https://www.langchain.com/)
* [OpenAI](https://openai.com/)
* [FAISS](https://github.com/facebookresearch/faiss)
