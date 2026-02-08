# 🚀 AI-Powered Resume Job Matching System

An end-to-end **AI-driven Resume Parser & Job Matching Dashboard** that extracts skills from resumes, compares them against real-world job descriptions, and ranks job opportunities using **LLM-powered ATS analysis**.

Built with **production-grade security**, **ML best practices**, and **interactive visual analytics**.

---

## 📌 Features

### 🔍 Resume Intelligence
- PDF text extraction with **OCR fallback**
- NLP-based **skill extraction & normalization**
- Skill confidence scoring based on frequency
- ATS-friendly resume reformatting using LLMs

### 🤖 AI Job Matching
- Real-time job fetching using **JSearch API**
- Resume ↔ Job comparison via **Groq LLM**
- ATS-style **match score (0–100)**
- Matching skills vs missing skills analysis
- Intelligent job recommendations: **Apply / Consider / Skip**

### 📊 Visual Analytics Dashboard
- Job match score bar charts
- Skills gap comparison
- Recommendation distribution (donut chart)
- Ranked job summary table
- Detailed job-wise analysis cards

### 🔐 Security & Reliability
- API keys handled via **environment variables**
- No hardcoded secrets
- Job search caching to avoid rate limits
- Graceful fallback if LLM fails
- Production-ready error handling

---

## 🧠 Tech Stack

| Category | Tools |
|--------|------|
| Language | Python 3.10+ |
| NLP | spaCy |
| OCR | Tesseract, pdf2image |
| LLM | Groq (LLaMA 3.3 – 70B) |
| APIs | JSearch (RapidAPI) |
| UI | Gradio |
| Visualization | Plotly |
| Data | Pandas |

---

## 🏗️ System Architecture

```
Resume PDF
↓
Text Extraction (PDF / OCR)
↓
Skill Extraction + Normalization
↓
AI Resume Formatting (Groq LLM)
↓
Job Fetching (JSearch API)
↓
Resume ↔ Job ATS Analysis (Groq LLM)
↓
Ranking + Recommendations
↓
Interactive Dashboard (Gradio + Plotly)
```


---

## 🔐 API Key Setup (IMPORTANT)

⚠️ **Never hardcode API keys**

### Google Colab
```python
import os

os.environ["RAPIDAPI_KEY"] = "your_rapidapi_key"
os.environ["GROQ_API_KEY"] = "your_groq_api_key"
```
### Local / Linux / Mac
```
export RAPIDAPI_KEY="your_rapidapi_key"
export GROQ_API_KEY="your_groq_api_key"
```

## 🧪 Example Use Cases

- Students applying for internships
- Freshers optimizing resumes for ATS
- Job seekers prioritizing best-fit roles
- Career guidance & resume analysis platforms
- Recruitment intelligence dashboards

---
## 🚀 Future Enhancements

- Resume ↔ Job embedding similarity scoring
- Personalized skill learning roadmap
- Resume ATS optimization suggestions
- Multi-resume comparison
- FastAPI backend + Docker deployment
- AWS / GCP production deployment
- Recruiter-side dashboard

---
