# 🤖 LLMOps & AIOps Project 8: RAG Medical Chatbot

![LLMOps](https://img.shields.io/badge/LLMOps-AIOps-blueviolet)
![Python](https://img.shields.io/badge/Python-3.12%2B-brightgreen)
![Docker](https://img.shields.io/badge/Docker-Ready-blue)
![Kubernetes](https://img.shields.io/badge/Kubernetes-Deploy-blue)
![License](https://img.shields.io/badge/License-GPL--3.0-orange)

A next-generation, Retrieval-Augmented Generation (RAG) Medical Chatbot designed for highly accurate medical Q&A. Built with modern LLMOps and AIOps best practices, this project leverages vector search, modular pipeline, Docker, Jenkins for CI/CD, and is ready for production and research deployments.

> 📁 **Repository:** `LLMOPS-AIOPS-Project8-RAG-MEDICAL-CHATBOT`

---

## 🚀 Project Highlights

- 🏥 **Medical RAG Chatbot:**  
  Ask medical questions and get accurate, context-aware answers using RAG (Retrieval Augmented Generation) pipelines.
- 🔎 **Vector Search:**  
  Fast semantic retrieval from medical encyclopedias (e.g., Gale Encyclopedia of Medicine).
- 🏗️ **Modular Pipeline:**  
  Components for loading, embedding, retrieval, and LLM-based answer generation.
- 🐳 **Dockerized:**  
  Build and run anywhere with ease.
- ☸️ **Kubernetes-Ready:**  
  Infrastructure as code for scalable, resilient deployment.
- 🔄 **CI/CD with Jenkins:**  
  Automated build, test, and deployment with Jenkinsfile.
- 📑 **Extensive Documentation:**  
  See `FULL_DOCUMENTATION.md` for technical and usage details.

---

## 🧠 Technical Stack

- **Python 3.12+**
- **FAISS** (Facebook AI Similarity Search for vector DB)
- **LLMs (OpenAI, etc.)** for answer generation
- **PDF, Data Loaders** for ingesting medical knowledge
- **Docker, Kubernetes, Jenkins**
- **Modern Python OOP & Pipeline Patterns**

---

## 🏗️ Project Structure

```bash
LLMOPS-AIOPS-Project8-RAG-MEDICAL-CHATBOT/
├── app/
│   ├── __init__.py
│   ├── application.py              # Main API/app entry point
│   ├── common/
│   │   ├── __init__.py
│   │   ├── custom_exception.py
│   │   └── logger.py
│   ├── components/
│   │   ├── __init__.py
│   │   ├── data_loader.py
│   │   ├── embeddings.py
│   │   ├── llm.py
│   │   ├── pdf_loader.py
│   │   ├── retriever.py
│   │   └── vector_store.py
│   ├── config/
│   │   ├── __init__.py
│   │   └── config.py
│   ├── templates/
│   │   └── __init__.py
├── vectorstore/
│   └── db_faiss/
│       ├── index.faiss             # Vector index
│       └── index.pkl
├── data/
│   └── The_GALE_ENCYCLOPEDIA_of_MEDICINE_SECOND.pdf
├── Dockerfile
├── Jenkinsfile
├── requirements.txt
├── setup.py
├── LICENSE
├── README.md
├── FULL_DOCUMENTATION.md
```

---

## ⚡ Installation & Usage

### 1. Clone the repository
```bash
git clone https://github.com/mdzaheerjk/LLMOPS-AIOPS-Project8-RAG-MEDICAL-CHATBOT.git
cd LLMOPS-AIOPS-Project8-RAG-MEDICAL-CHATBOT
```

### 2. Set up a virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the application
```bash
python app/application.py
```
Or build and run with Docker:
```bash
docker build -t rag-medical-chatbot .
docker run -p 8000:8000 rag-medical-chatbot
```

### 5. Kubernetes Deployment
(You may need to adapt a manifest for your cluster.)

### 6. CI/CD with Jenkins
See `Jenkinsfile` for pipeline automation.

---

## 🧪 Example Usage

- **Medical Q&A:**  
  Ask questions like "What is hypertension?", "Symptoms of diabetes?", etc., to get accurate, sourced, context-rich answers from medical knowledge bases.
- **Semantic Search:**  
  The chatbot retrieves evidence from encyclopedic sources, then uses LLMs to generate responses.

---

## 📚 Documentation

See [FULL_DOCUMENTATION.md](FULL_DOCUMENTATION.md) for detailed architecture, RAG pipeline, and configuration instructions.

---

## ✍️ Author

**Mohammed Zaheeruddin**  
🎓 First-Year B.Tech Student | AI/ML & GenAI Enthusiast  
🏫 Shetty Institute of Technology, Gulbarga  
📧 info.zaheerjk@gmail.com

---

## 📜 License

This project is licensed under the **GPL-3.0 License** – see the LICENSE file for details.

---

#### Key Features:
1. RAG pipeline for evidence-based, LLM-powered medical Q&A
2. Modular, extensible codebase with vector search and PDF ingestion
3. Docker, Jenkins, and Kubernetes for production and research scale
4. Designed for medical research, education, and real-world deployment
