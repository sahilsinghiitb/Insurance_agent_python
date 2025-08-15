## 🤖 Virtual Insurance Agent using LangChain & Together AI  
 

This project involves building a Retrieval-Augmented Generation (RAG) based chatbot that can answer insurance-related questions by leveraging a knowledge base made from insurance exam PDFs.

---

### 🧾 Objective
To develop a conversational agent capable of answering insurance domain queries using AI, by combining language models with a document-based vector database for accurate retrieval and generation.

---

### 🗃️ Data & Preprocessing
- Collected **insurance exam PDFs** and loaded them using **PyPDFLoader**
- Split documents into manageable chunks using **RecursiveCharacterTextSplitter**
- Generated **sentence embeddings** using SentenceTransformers

---

### 🧠 Model Architecture (RAG Pipeline)
- Stored embeddings in a **ChromaDB vector store** for semantic retrieval
- Built a **RetrievalQA chain** using **Together AI** LLM integrated via LangChain
- Created a **custom prompt template** for more domain-specific and concise answers

---

### ✅ Results & Features
- End-to-end pipeline returns accurate answers to insurance queries pulled from PDF knowledge base
- Built a simple conversational interface using **Gradio** for real-time interaction
- Demonstrated strong context awareness and domain-specific relevance using RAG retrieval

---

### 🚀 Deployment & Future Scope
- Deployed locally via **Gradio UI**, can be extended to Flask / FastAPI for production use
- Future improvements: conversational memory, more documents, auto fine-tuning, integration with external APIs

---

### 🛠️ Tools & Libraries
- Python, LangChain, ChromaDB, SentenceTransformers, Together AI, Gradio, PyPDFLoader
