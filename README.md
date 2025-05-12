# 🤖 CTSE Lecture Notes ChatBot

This project is an intelligent academic assistant that answers software engineering questions using **only the CTSE lecture slides**. It leverages modern NLP techniques like Retrieval-Augmented Generation (RAG), sentence-transformer embeddings, and instruction-tuned LLMs like **FLAN-T5**.

---

## 📌 Features

- 🔍 Answers are generated using your **CTSE lecture PDFs** only (no external data).
- 📚 Semantic search with **ChromaDB** and **MiniLM** embeddings.
- 🧠 Natural language generation via **FLAN-T5-large** (from HuggingFace).
- ✅ Responses are clean, formal, and limited to ~100 words.
- 💬 Future support for UI using Gradio.

---

## 🛠️ Tech Stack

- `LangChain` – Orchestration of retrieval + generation
- `ChromaDB` – Vector database for document chunks
- `sentence-transformers/all-MiniLM-L6-v2` – Text embedding model
- `FLAN-T5-large` – Pre-trained instruction-following LLM
- `PyPDFLoader` – Extracts content from lecture PDFs
- `Python` (Jupyter Notebook or VS Code)

---

## 🚀 How to Run

1. Clone the repository  
```

git clone [https://github.com/your-username/ctse\_chatbot](https://github.com/your-username/ctse_chatbot)
cd ctse\_chatbot

```

2. Install dependencies  
```

pip install -r requirements.txt

```

3. Place your **lecture slides** (PDFs) inside the `/lecture_notes` folder.

4. Open `ChatBot.ipynb` and run all cells to:
- Load documents
- Create embeddings
- Build the QA chain
- Ask questions using `ask_detailed("Your Question")`

---


## 👨‍💻 Author

Developed by [Your Name] – University of Sri Lanka Institute of Information Technology (SLIIT) – SE4010 AI/ML Assignment.
```

---

