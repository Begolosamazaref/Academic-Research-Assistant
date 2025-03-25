# Academic-Research-Assistant

This project is an **AI-powered academic research assistant** that fetches and summarizes research data from **Wikipedia** and **Arxiv**, processes it using **Groq's AI models**, and generates structured reports.

---

## 📌 Features
- Fetches research data from **Wikipedia** and **Arxiv**
- Summarizes large documents in **chunks**
- Filters **relevant** insights
- Generates a structured **research report**

---

## 🚀 Installation

First, install the required dependencies:
```bash
pip install faiss-cpu langchain langchain-community langchain-groq transformers sentence-transformers wikipedia wikipedia-api pymupdf arxiv
```

---

## 🔑 Setting Up API Key

This project requires a **Groq API key** for processing research data. Set it up as an environment variable:

```bash
export GROQ_API_KEY="your_api_key_here"
```
Or enter it when prompted during runtime.

---

## 📄 Usage

Run the script and enter a research topic:
```bash
python research_assistant.py
```

### **Example Input**
```
Enter a research topic: cloud
```

### **Example Output**
```json
{
    "query": "cloud",
    "sources": [
        "Wikipedia (cloud)",
        "Arxiv (cloud)"
    ],
    "summary": "Extracted key insights from Wikipedia and Arxiv sources...",
    "filtered_research": "Refined summary focusing on the most relevant aspects..."
}
```

---

## 📜 How It Works

1. **Fetch Research Data** → Retrieves **Wikipedia & Arxiv** documents
2. **Process in Chunks** → Splits content to avoid token limits
3. **Filter Relevant Info** → AI extracts **essential insights**
4. **Generate Research Report** → Outputs a **structured JSON report**

---
