⭐ Daily CNN-Based MRI Deep Learning Research Aggregator & Summarizer (n8n)
======================================================================

An automated **n8n research intelligence workflow** that runs daily to discover, aggregate, filter, and summarize **recent MRI-focused deep learning research** using CNNs. The system queries multiple academic sources, extracts metadata and full text where available, stores results for longitudinal tracking, and sends daily notifications.

⭐ Workflow File  
Daily CNN-Based MRI Deep Learning Research Aggregator and Summarizer.json

---

⭐ Key Features
---------------

⭐ Daily scheduled execution (08:00 EST)  
⭐ Multi-source academic search (PubMed, arXiv, CrossRef)  
⭐ Advanced keyword-based filtering for MRI + CNN research  
⭐ Automatic PDF download and text extraction  
⭐ Centralized storage in Google Sheets  
⭐ Daily Slack summary notifications  
⭐ Error handling and logging  

---

⭐ System Architecture
---------------------

Daily Scheduler  
   ↓  
Search Configuration  
   ↓  
PubMed / arXiv / CrossRef APIs  
   ↓  
Metadata Parsing & Normalization  
   ↓  
MRI + CNN Keyword Filtering  
   ↓  
PDF Download & Text Extraction  
   ↓  
Google Sheets Storage  
   ↓  
Slack Notification  

---

⭐ Workflow Logic
----------------

⭐ Daily Trigger  
Runs automatically every morning at 08:00 EST.

⭐ Search Configuration  
Defines:
- Lookback window (e.g., last 14 days)
- Search terms for MRI + CNN + deep learning

⭐ Multi-Source Querying  
Fetches recent papers from:
- PubMed  
- arXiv  
- CrossRef  

⭐ Parsing & Normalization  
Extracts:
- Title  
- Abstract  
- Authors  
- DOI  
- Publication date  
- Journal / source  
- Keywords  

⭐ Intelligent Filtering  
Keeps only papers containing:
- MRI or magnetic resonance imaging  
- CNN or convolutional neural networks  
- Deep learning  

⭐ PDF Processing  
- Downloads full-text PDFs when available  
- Extracts readable text for downstream analysis  

⭐ Data Persistence  
Stores structured metadata and extracted text into Google Sheets for tracking and review.

⭐ Aggregation & Notification  
Compiles a daily summary and sends a Slack notification listing newly processed papers.

⭐ Error Logging  
Captures failed downloads, parsing issues, and invalid records in a separate error log sheet.

---

⭐ Data Stored Per Paper
-----------------------

| ⭐ Field | ⭐ Description |
|-------|--------------|
| title | Paper title |
| abstract | Abstract or summary |
| authors | Author list |
| doi | DOI or arXiv ID |
| publicationDate | Publication date |
| journalName | Journal or source |
| link | Paper or PDF link |
| keywords | Extracted keywords |
| source | PubMed / arXiv / CrossRef |
| fullText | Extracted PDF text |

---

⭐ External Integrations
-----------------------

⭐ PubMed API  
⭐ arXiv API  
⭐ CrossRef API  
⭐ Google Sheets (storage + logging)  
⭐ Slack (daily notifications)

---

⭐ Credentials Required
----------------------

⭐ Google Sheets OAuth2  
Read/write access for storage and error logging

⭐ Slack OAuth2  
Permission to send daily summary messages

---

⭐ Getting Started
-----------------

⭐ Import the workflow JSON into n8n  
⭐ Configure Google Sheets and Slack credentials  
⭐ Review search terms and lookback window  
⭐ Verify target Google Sheets IDs  
⭐ Activate the workflow  

---

⭐ Customization Options
-----------------------

⭐ Adjust lookback window (daysBack)  
⭐ Expand or refine keyword filters  
⭐ Add OpenAI / LLM-based summarization  
⭐ Export results to a database or vector store  
⭐ Add email notifications in addition to Slack  

---

⭐ Use Cases
-----------

⭐ Academic research monitoring  
⭐ Medical imaging literature review  
⭐ AI/ML research tracking  
⭐ Graduate or undergraduate research support  
⭐ Personal research intelligence automation  

---

⭐ Why This Project Stands Out
-----------------------------

⭐ Demonstrates real-world research automation  
⭐ Multi-API orchestration and parsing  
⭐ Full-text PDF processing at scale  
⭐ Robust filtering and fault tolerance  
⭐ Practical application of AI research workflows  

Ideal for **GitHub portfolios, research showcases, internships, and college applications**.

---

⭐ License
---------

This project is intended for educational, research, and internal use.  
You are free to modify and extend it for your own workflows.
