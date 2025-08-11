[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/vgbm4cZ0)

Folder Structure

ai-engineer-assignment/
├── app.py
├── requirements.txt
├── README.md
├── samples/
│   ├── sample_missing_adgm.docx
│   ├── sample_all_rules_ok.docx
└── output_demo/
    ├── reviewed_sample_missing_adgm.docx
    ├── reviewed_sample_all_rules_ok.docx
    └── report.json


requirements.txt

gradio==4.29.0
python-docx==1.1.0


README.md
# ADGM Corporate Agent - Document Reviewer

This application reviews `.docx` documents for compliance with specific ADGM corporate agent requirements.

## Features
- Checks if "ADGM" jurisdiction is mentioned.
- Verifies placeholders for:
  - Company Name
  - Registered Address
  - Signature Section
  - Date
- Adds reviewer comments to the end of each document.
- Generates a JSON report summarizing all issues.

---

## Setup Instructions

### Step 1 — Create Virtual Environment
```bash
python -m venv venv

Step 2 — Activate Environment
Windows (PowerShell):
venv\Scripts\Activate.ps1

macOS/Linux:
source venv/bin/activate

Step 3 — Install Dependencies
pip install -r requirements.txt

Running the App
python app.py

You will see a local URL like:
Running on local URL: http://127.0.0.1:7860
Open it in your browser.