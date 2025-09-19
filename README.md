# RAG_pipeline

A **Retrieval-Augmented Generation (RAG)** pipeline that retrieves relevant documents and generates answers grounded in those documents.

---

## 📌 Overview

This project implements a simple RAG pipeline that combines **document retrieval** with **language generation**.  
It can be used for:

- Question Answering  
- Knowledge-based chat assistants  
- Summarization with context  
- Domain adaptation of LLMs  

---

## 🚀 Features

- Document ingestion and retrieval  
- Support for configurable top-k retrieval  
- Generative model integration  
- Modular structure for easy extension  
- Example notebooks for exploration  

---

## 📂 Repository Structure

RAG_pipeline/
├── data/                ← Document corpus, example data  
├── notebooks/           ← Jupyter notebooks for experiments  
├── main.py              ← Entry-point for running pipeline  
├── requirements.txt     ← Python dependencies  
├── pyproject.toml       ← Project configuration & packaging  
├── .python-version       ← Python version specification  
├── README.md            ← This file  
└── .gitignore           ← Files/folders to ignore in version control  



---

## ⚙️ Installation

1. Clone the repository:

```bash
git clone https://github.com/Thirumal-iith/RAG_pipeline.git
cd RAG_pipeline


python3 -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

pip install -r requirements.txt

## ▶️ Usage

Run the pipeline with:

python main.py --query "Your question here" --top_k 5


Arguments:

Flag	Description	Default
--query	Input question/query text	required
--top_k	Number of documents to retrieve	5
--doc_path	Path to document corpus	data/
--model	Generative model to use	e.g. gpt

