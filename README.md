# 📊 Data Extraction & Integration — Factors Export Tool

A cloud-based Python automation tool that logs into Factors.ai, extracts account-level insights, captures dashboard screenshots, and exports both structured data and visuals to Google Sheets and Google Drive.  
It also uses Ollama + Mistral to organize unstructured text into meaningful fields.

---

## 💡 Features

- Logs into the Factors.ai dashboard with secure credentials
- Navigates to each account's overview and timeline pages
- Extracts:
  - Company name, domain, industry, revenue, location
  - Traffic data, timeline events, top pages, and engagement
- Captures high-resolution screenshots of:
  - Overview metrics
  - Timeline activity for each account
- Uploads data and screenshots to:
  - 📄 Google Sheets (structured format)
  - 🖼️ Google Drive (organized folders)
- Uses **Ollama + Mistral** to clean and format raw text before export
- Supports headless cloud execution with daily scheduling via cron

---

## 🛠 Technologies

- Python 3
- Playwright (browser automation)
- Google Sheets API
- Google Drive API
- Ollama + Mistral LLM (local AI inference)
- Docker (for cloud deployment)
- Cron (for task scheduling)

---

## ⚙️ Architecture

1. Authenticates into Factors.ai
2. Paginates through the account list
3. For each account:
   - Opens overview and timeline
   - Extracts structured and raw text data
   - Parses unstructured fields with Ollama (Mistral model)
   - Takes screenshots
4. Uploads data to Google Sheets
5. Uploads screenshots to Google Drive in a per-company folder

---

## 🚀 Deployment Options

- Google Cloud Run with Docker
- Virtual Machine (cron-based)
- Any cloud server supporting Python and headless browsers

---

## 🔐 Access

🔒 Source code is private.  
This repository provides a public overview of the project scope and functionality.

---

## 🧑‍💻 Author

**TrkElnIt** – Cloud automation, LLM pipelines, and data workflows  

