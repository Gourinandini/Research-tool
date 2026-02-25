# 🔎 Research Tool

An AI-powered research assistant that helps users discover, explore, and interact with academic papers and code repositories. The tool integrates **arXiv search**, **GitHub search**, **PDF preview**, **question answering**, and **LLM-based analysis** into a unified Streamlit interface.

---

## ✨ Features

### 📄 arXiv Paper Search

* Search academic papers by topic
* Retrieve title, summary, authors, publication date, and URL
* Relevance-based sorting

### 💻 GitHub Repository Search

* Discover repositories related to research topics
* View repository metadata and links

### 📑 PDF Preview

* Inline paper preview inside the app
* Seamless reading without downloading

### ❓ PDF Question Answering

* Ask questions about research papers
* Context-aware answers using LLM

### 🤖 Local LLM Integration

* Uses a fine-tuned TinyLLaMA (QLoRA)
* Supports offline inference

### 🎛️ Streamlit UI

* Clean multi-page interface
* Interactive research workflow

---

## 🏗️ Project Structure

```
Research-tool/
│
├── app.py
├── requirements.txt
├── README.md
│
├── components/
│   ├── arxiv_search.py
│   └── github_search.py
│
├── pages/
│   └── components/
│       ├── pdf_preview.py
│       ├── pdf_qa_engine.py
│       ├── view_paper.py
│       └── my_model.py
│
└── .streamlit/
    └── secrets.toml
```

---

## ⚙️ Installation

### 1️⃣ Clone the repository

```
git clone <repo-url>
cd Research-tool
```

### 2️⃣ Create virtual environment

```
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows
```

### 3️⃣ Install dependencies

```
pip install -r requirements.txt
```

---

## ▶️ Running the App

```
streamlit run app.py
```

The application will open in your browser.

---

## 🔑 Environment Variables

Create `.env` or `.streamlit/secrets.toml` for API keys if required:

```
GITHUB_TOKEN=your_token
GROQ_API_KEY=your_key
```

---

## 🧠 How It Works

1. User searches topic
2. arXiv API fetches research papers
3. GitHub search finds related code
4. PDF loader extracts text
5. QA engine builds embeddings
6. Fine-tuned LLM generates answers

---

## 🚀 Tech Stack

* Python
* Streamlit
* arXiv API
* GitHub API
* LangChain
* QLoRA Fine-tuning
* TinyLLaMA
* Groq API (optional)

---

## 📌 Future Improvements

* Semantic paper recommendation
* Citation graph visualization
* Multi-paper comparison
* RAG optimization
* Research notes export

---

## 👩‍💻 Author

**Gourinandini Sunil**

---

## ⭐ Contribution

Contributions are welcome! Feel free to fork, open issues, or submit pull requests.

---

## 📜 License

This project is for educational and research purposes.
