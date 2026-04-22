# 🚀 InvoiceIQ — AI-Powered Invoice Processing System

InvoiceIQ is an end-to-end AI system that automates invoice processing using Large Language Models (LLMs). It extracts structured data from PDFs, validates financial correctness, prevents duplicates, and provides real-time analytics through an interactive dashboard.

---

## ✨ Features

* 📄 **PDF Invoice Parsing** — Extracts raw text from invoices using PyMuPDF
* 🤖 **AI Data Extraction** — Uses Groq (LLaMA 3) to convert unstructured text into structured JSON
* ✅ **Validation Engine** — Ensures correctness (GST checks, missing fields, anomaly detection)
* 🔁 **Duplicate Detection** — Prevents re-processing of invoices
* 🗄️ **Database Storage** — Stores structured invoice data using SQLite + SQLAlchemy
* 🌐 **FastAPI Backend** — Simulated ERP endpoint for invoice submission
* 📊 **Modern Dashboard** — Streamlit UI with analytics and insights
* 🧠 **AI Summary Generator** — Generates business-level insights from invoice data

---

## 🧠 System Architecture

```
PDF → Parser → LLM Extractor → Validator → Duplicate Checker → Database → API → Dashboard → AI Summary
```

---

## 🛠️ Tech Stack

* **Language:** Python
* **LLM:** Groq (LLaMA 3)
* **AI Orchestration:** LangChain
* **PDF Processing:** PyMuPDF
* **Backend:** FastAPI
* **Database:** SQLite + SQLAlchemy
* **Frontend:** Streamlit
* **Validation:** Pydantic

---

## 📁 Project Structure

```
InvoiceIQ/
├── app.py                 # Streamlit dashboard
├── api.py                 # FastAPI backend (ERP simulation)
├── parser.py              # PDF text extraction
├── extractor.py           # LLM-based data extraction
├── validator.py           # Data validation engine
├── duplicate_checker.py   # Duplicate detection
├── database.py            # Database layer (SQLAlchemy)
├── summary.py             # AI summary generator
├── sample_invoices/       # Test invoices
├── requirements.txt
├── .env
└── README.md
```

---

## ⚙️ Setup Instructions

```bash
# Clone repo
git clone https://github.com/your-username/InvoiceIQ.git
cd InvoiceIQ

# Create virtual environment
python -m venv venv
venv\Scripts\activate   # Windows

# Install dependencies
pip install -r requirements.txt
```

### 🔑 Add Groq API Key

Create a `.env` file:

```
GROQ_API_KEY=your_api_key_here
```

---

## ▶️ Run the Project

### 1. Start API Server

```bash
uvicorn api:app --reload
```

### 2. Run Dashboard

```bash
streamlit run app.py
```

### 3. Test Pipeline

```bash
python summary.py
```

---

## 📊 Example Output

* Structured invoice data (JSON)
* Validation results
* Duplicate detection alerts
* Dashboard with metrics + charts
* AI-generated financial summaries

---

## 🚀 Future Improvements

* OCR support for scanned invoices
* Drag & drop upload UI
* AI chat interface for invoice querying
* Cloud deployment (AWS / GCP)
* Real ERP integration

---

## 👨‍💻 Author

**Anuj Wankhede**
B.Tech IT | AI/ML Enthusiast

```
```
