# 📄 Chat with PDF using RAG | Mistral AI + LangChain + ChromaDB

An AI-powered Retrieval-Augmented Generation (RAG) application that allows users to upload PDF documents and chat with them using Mistral AI. The application extracts relevant information from the uploaded document and answers user questions based only on the document's content.

---

## 🚀 Features

- 📂 Upload any PDF document
- 🤖 Chat with the uploaded PDF
- 🔍 Semantic search using Hugging Face Embeddings
- 🧠 Retrieval-Augmented Generation (RAG)
- 📚 Source-aware responses
- 💬 Interactive chat interface using Streamlit
- ⚡ Fast document retrieval with ChromaDB
- 🔒 Environment variable support using `.env`

---

## 🛠️ Tech Stack

### Frontend
- Streamlit

### Backend
- Python

### LLM
- Mistral AI (`mistral-small-2506`)

### Framework
- LangChain

### Embedding Model
- BAAI/bge-base-en-v1.5

### Vector Database
- ChromaDB

### Document Loader
- PyPDFLoader

### Text Chunking
- RecursiveCharacterTextSplitter

---

## 📁 Project Structure

```text
RAG_PROJECT/
│
├── app.py
├── .env
├── requirements.txt
├── chroma_db/
├── uploads/
└── assets/
```

---

## ⚙️ Installation

### Clone the repository

```bash
git clone https://github.com/yourusername/rag-chatbot.git

cd rag-chatbot
```

### Create Virtual Environment

Using uv

```bash
uv venv
```

Activate

Windows

```bash
.venv\Scripts\activate
```

Linux / macOS

```bash
source .venv/bin/activate
```

---

### Install dependencies

```bash
uv pip install -r requirements.txt
```

or

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

Create a `.env` file in the project root.

```env
MISTRAL_API_KEY=YOUR_API_KEY
```

---

## ▶️ Run the Application

```bash
streamlit run app.py
```

---

## 🧠 How It Works

1. User uploads a PDF.
2. The PDF is loaded using PyPDFLoader.
3. The document is split into smaller chunks.
4. Each chunk is converted into vector embeddings using Hugging Face BGE embeddings.
5. The embeddings are stored inside ChromaDB.
6. When a user asks a question:
   - Relevant chunks are retrieved.
   - Retrieved context is passed to Mistral AI.
   - The model generates an answer based only on the retrieved context.

---

## 📷 Screenshots

### Upload PDF

Add screenshot here

```
assets/upload.png
```

### Chat Interface

Add screenshot here

```
assets/chat.png
```

---

## 📦 Dependencies

- LangChain
- LangChain Chroma
- LangChain HuggingFace
- LangChain MistralAI
- ChromaDB
- Streamlit
- Mistral AI
- Hugging Face Sentence Transformers
- PyPDF
- Python Dotenv

---

## 💡 Future Improvements

- Support multiple PDFs
- Persistent vector database
- Streaming responses
- Chat history memory
- PDF page preview
- Citation highlighting
- OCR support for scanned PDFs
- Multi-user authentication
- Dark mode UI
- Docker deployment
- Cloud deployment (Render/AWS)

---

## 🎯 Learning Outcomes

This project demonstrates:

- Retrieval-Augmented Generation (RAG)
- Large Language Model integration
- Vector Databases
- Embedding Models
- Semantic Search
- Prompt Engineering
- LangChain Pipelines
- Streamlit Application Development

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Swapnil**

Computer Engineering Student

Interested in:

- Artificial Intelligence
- Machine Learning
- Generative AI
- Full Stack Development

---

⭐ If you found this project useful, consider giving it a star!
