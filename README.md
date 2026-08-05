
# MITA — Multimodal Industrial Troubleshooting Assistant

A smart fault diagnosis system for industrial machines that combines 
Computer Vision, Voice Recognition, and RAG (Retrieval-Augmented Generation) 
to provide accurate, grounded troubleshooting guidance.

> Built as a Major Project by a group of 4 students.

---

## 🔍 What It Does

A technician can:
- 📷 Upload a photo of a faulty machine
- 🎙️ Describe the fault by voice
- ⌨️ Type a query or fault code

The system analyzes all three inputs, searches a knowledge base of 
machine manuals and fault logs, and generates step-by-step repair instructions.

---

## 🏗️ System Architecture

User Input (Image + Voice + Text)
        ↓
FastAPI Backend
        ↓
Vision (CLIP + YOLO) | Voice (Whisper STT) | Text Processing
        ↓
Query Fusion Module
        ↓
RAG Pipeline (ChromaDB Vector Search)
        ↓
LLM Answer Generation (GPT-4o)
        ↓
Step-by-step Troubleshooting Response

---

## 🛠️ Tech Stack

| Layer        | Technology                        |
|--------------|-----------------------------------|
| Frontend     | React + Tailwind CSS              |
| Backend      | FastAPI (Python)                  |
| Voice / STT  | OpenAI Whisper                    |
| Vision       | CLIP + YOLOv8                     |
| Embeddings   | sentence-transformers             |
| Vector DB    | ChromaDB                          |
| LLM          | GPT-4o                            |
| Orchestration| LangChain                         |
| Deployment   | Docker                            |

---


## 👥 Team

| Name         | Role                        |
|--------------|-----------------------------|
| Member 1     | Backend + RAG Pipeline      |
| Member 2     | Vision Module (CLIP + YOLO) |
| Member 3     | Voice Module + Prompt Eng.  |
| Member 4     | Frontend + Deployment       |

---

## 📊 Evaluation Metrics

| Metric                  | Target  |
|-------------------------|---------|
| STT Word Error Rate     | < 10%   |
| RAG Retrieval Precision | > 80%   |
| Answer Accuracy         | > 75%   |
| Response Latency        | < 8 sec |

---

## 🔮 Future Scope

- Real-time video feed analysis
- Voice output (Text-to-Speech)
- Edge deployment on factory tablets
- Fault analytics dashboard
- Multilingual support

---

## 📄 License

MIT License — free to use for academic purposes.
