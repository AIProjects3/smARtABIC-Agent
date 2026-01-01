# smARtABIC-Agent

An Arabic Retrieval-Augmented Generation (RAG) system for Arabic Question Answering.

This project retrieves relevant Arabic knowledge using semantic search (FAISS + E5 embeddings) and generates grounded answers for user queries.

---

## ✨ Features

- Arabic semantic retrieval using E5 embeddings  
- FAISS vector search  
- Robust handling of unknown questions  
- Fully offline deployment  
- Interactive Web Interface  

---

## 📊 Dataset

We use a cleaned Arabic QA dataset split into training and evaluation subsets.  
The system was evaluated on unseen validation samples.

---

## 🛠 Requirements

1. Python **3.9** or higher  
2. `pip`

---

## 📥 Installation

1. Download the project or clone it:

```bash
git clone https://github.com/EngMar26/smARtABIC-Agent.git
cd smARtABIC-Agent

2.Install required libraries:
   pip install -r requirements.txt

---

▶️ How to Run the System

From the project folder, run:
  python -m uvicorn app.server:app --host 127.0.0.1 --port 8000

Then open your browser at:
   http://127.0.0.1:8000

You can now ask questions in Arabic.

---

🌐 Offline Usage
This system works fully offline after installation:
 All models and indices are stored locally
 No internet connection is required for answering questions
 Suitable for demonstrations and presentations without network access

---

📁 Project Structure
smARtABIC-Agent/
│
├── app/            # Backend and web interface
├── data/           # FAISS index, chunks, logo, assets
├── results/        # Evaluation results and screenshots
├── requirements.txt
└── README.md

---

🧪 Evaluation Summary
  Evaluation was performed on unseen validation samples.
    Recall@5 ≈ 0.23
    Recall@10 ≈ 0.30
    Don't-know rate ≈ 0.03

Screenshots of results are available in the results/ folder.

---

🎓 Graduation Project

This system represents the final submission version of the graduation project
titled:
smARtABIC: An Offline Arabic Retrieval-Augmented Intelligent Agent
