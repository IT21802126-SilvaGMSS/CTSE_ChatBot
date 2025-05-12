# 🤖 CTSE Lecture Notes ChatBot

This project is an intelligent academic assistant that answers software engineering questions using **only the CTSE lecture slides**. It leverages modern NLP techniques like Retrieval-Augmented Generation (RAG), sentence-transformer embeddings, and instruction-tuned LLMs like **FLAN-T5**.

---

## 📌 Features

- 🔍 Answers are generated using your **CTSE lecture PDFs** only (no external data)
- 📚 Semantic search with **ChromaDB** and **MiniLM** embeddings
- 🧠 Natural language generation via **FLAN-T5-large** (from HuggingFace)
- ✅ Responses are clean, formal, and limited to ~100 words
- 💬 Optional Gradio-based UI (future enhancement)

---

## 🛠️ Tech Stack

- `LangChain` – Orchestration of retrieval + generation
- `ChromaDB` – Vector database for document chunks
- `sentence-transformers/all-MiniLM-L6-v2` – Text embedding model
- `FLAN-T5-large` – Instruction-tuned LLM for structured answers
- `PyPDFLoader` – For extracting text from lecture PDFs
- `Python` – Executed via Jupyter Notebook or VS Code

---

## 🚀 How to Run

1. **Clone the repository**

```bash
git clone https://github.com/your-username/ctse_chatbot
cd ctse_chatbot
````

2. **Install dependencies**

```bash
pip install -r requirements.txt
```

3. **Add lecture PDFs**

Place your **lecture slides** inside the `lecture_notes/` folder.

4. **Launch notebook**

Open `ChatBot.ipynb` and run all cells to:

* Load lecture documents
* Split and embed text
* Store chunks in ChromaDB
* Ask questions with `ask_detailed("Your Question")`

---

## 👨‍💻 Author

Developed by **Silva G M S S**
Department of Software Engineering – SLIIT
*SE4010 AI/ML Individual Assignment*
