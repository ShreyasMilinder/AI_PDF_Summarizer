# 🛡️ AI PDF Cybersecurity Summarizer (Local LLM)
An **AI-powered cybersecurity document summarization tool** that analyzes multiple client PDF reports, correlates findings, and automatically generates a **professional, presentation-ready PowerPoint (PPT)** — all **locally**, without sending data to the cloud. 
Built using Mistral LLM via Ollama, this project is ideal for SOC analysts, SIEM engineers, and cybersecurity teams who handle sensitive client data.

## 🚀 Key Features

- 📄 **Summarizes multiple cybersecurity PDFs**
- 🧠 **Correlates findings across clients**
- 📊 **Generates a single executive-ready PPT**
- 🔐 **100% local processing (no cloud, no data leakage)**
- 🪄 **Automatic slide splitting & clean formatting**
- ⚡ **8Uses open-source LLM (Mistral) via Ollama**

---

## 🧱 Architecture Overview

### PDF Reports
↓
### PDF Text Extraction (pdfplumber)
↓
### Local LLM (Mistral via Ollama)
↓
### AI Summaries + Correlation
↓
### Formatted PowerPoint Report (python-pptx)

## 🛠️ Tech Stack

- **Language: Python 3.x**
- **LLM: Mistral (via Ollama – local inference)**
- **PDF Parsing: pdfplumber**
- **Presentation Generation: python-pptx**
- **HTTP Client: requests**
- **Editor (recommended): Cursor / VS Code**


---

## 📂 Project Structure

├── summarize_to_ppt.py
├── requirements.txt
├── pdfs/ # Input PDFs (ignored by git)
├── .gitignore
└── README.md

---

## ⚙️ Prerequisites

- Python 3.10+
- Ollama installed
- Mistral model pulled locally

### Install Ollama & Model
```bash
ollama pull mistral
```

### Verify installation:
```bash
ollama run mistral
```
**(This will start an interactive session; type a message and press Enter to test. Exit with /bye or Ctrl+C.)**

---

## 📦 Installation

### Clone the repository:
```bash
git clone https://github.com/ShreyasMilinder/AI_PDF_Summarizer.git
cd AI_PDF_Summarizer
```

### Install dependencies:
```bash
pip install -r requirements.txt
```

---

## ▶️ How to Run

### 1. Place your cybersecurity PDFs inside the pdfs/ folder (Any filename works)
### 2. Run the script:
  ```bash
  python summarize_to_ppt.py
  ```
  
### 3. Output:
```bash
Cybersecurity_Summary_Report.pptx
```

***🎉 A clean, multi-slide, executive-ready PPT will be generated automatically.***

---

## 📊 PPT Output Includes

- **Title slide**
- **Individual client summaries**
    - **Threats**
    - **Vulnerabilities**
    - **Security incidents**
    - **Recommendations**
- **Correlated findings across all PDFs**
- **Overall risk assessment**
- **Unified security recommendations**
- **Automatic slide continuation for long content**

---

## 🔐 Security & Privacy

- **✅ No cloud APIs**
- **✅ No external data sharing**
- **✅ Suitable for SOC / MSSP / Enterprise environments**
- **✅ Client PDFs are excluded from GitHub via .gitignore**

---

## 📈 Use Cases

- **SOC incident reporting**
- **Client security assessment summaries**
- **MSSP executive reporting**
- **Internal risk analysis**
- **AI-assisted security documentation**

---

## 🧠 Resume Highlight

**Built a local LLM-based system using Mistral and Ollama to analyze, correlate, and auto-generate executive cybersecurity reports from multiple client PDFs.**

---

## 🚀 Future Enhancements

- **MITRE ATT&CK mapping**
- **Risk scoring (High / Medium / Low)**
- **Executive vs Technical PPT versions**
- **FastAPI REST service**
- **SIEM / Graylog integration**
- **Logo & branding support**

---

## 👤 Author

**Shreyas Milinder
Cybersecurity | SOC | AI Automation
GitHub: https://github.com/ShreyasMilinder
⭐ If you like this project
Give it a ⭐ on GitHub — it really helps!**


---

## ✅ How to Add This to GitHub
1. Create a file named **`README.md`** in your project root
2. Paste the above content
3. Commit & push:
```bash
git add README.md
git commit -m "Add project README"
git push
