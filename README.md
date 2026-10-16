# 🔍 NIC Code Semantic Search — Government Industry Classification via ModernBERT + FAISS

> Type a business description in plain English (or speak it) → instantly find the matching **National Industrial Classification (NIC) code** using semantic embeddings, not keyword matching.

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![ModernBERT](https://img.shields.io/badge/ModernBERT-nomic--ai-412991?style=flat-square)
![FAISS](https://img.shields.io/badge/FAISS-Vector_Search-00A67E?style=flat-square)

---

## 🎯 Overview

India's **NIC (National Industrial Classification)** system has thousands of industry codes used in government filings and business registration. Finding the right code manually is tedious. This project builds a **semantic search engine** over the entire NIC taxonomy — embedding all codes with `nomic-ai/modernbert-embed-base` and indexing them in FAISS for millisecond-latency similarity search.

---

## ✨ Features

- 🧠 **ModernBERT Embeddings** — state-of-the-art `nomic-ai/modernbert-embed-base` for semantic understanding
- ⚡ **FAISS Vector Index** — sub-millisecond nearest-neighbour search over full NIC taxonomy
- 🎙️ **Voice Input** — speech-to-text for hands-free code lookup
- 🔌 **FastAPI Backend** — RESTful API with top-k results and confidence scores
- 🌐 **Web Frontend** — clean UI with text and voice search modes

---

## 🛠️ Tech Stack

| Component | Technology |
|---|---|
| Embeddings | nomic-ai/modernbert-embed-base |
| Vector Search | FAISS |
| Backend | FastAPI |
| Frontend | HTML/CSS/JS |
| Language | Python 3.10+ |

---

## 🚀 Quick Start

```bash
git clone https://github.com/devcode-X/AI-Based-NIC-Code-Semantic-Search
cd AI-Based-NIC-Code-Semantic-Search
pip install -r requirements.txt

# Build the FAISS index (first time only)
python build_index.py

# Start the API server
uvicorn main:app --reload

# Open frontend
open index.html
```

---

## 📁 Structure

```
AI-Based-NIC-Code-Semantic-Search/
├── build_index.py       # Embeds NIC codes & builds FAISS index
├── main.py              # FastAPI search API
├── data/
│   └── nic_codes.csv    # NIC taxonomy data
├── static/              # Frontend assets
└── index.html           # Web UI
```
