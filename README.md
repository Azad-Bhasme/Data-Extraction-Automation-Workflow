# FAX EXTRACTION AUTOMATION WORKFLOW
📖 Project Overview

This project automates the extraction of fax numbers, phone numbers, and email IDs from law firm websites.
It uses Apify for LLM-powered scraping and N8N for workflow automation, data cleaning, and automatic storage into Google Sheets.

This project focuses on streamlining manual data collection into a seamless, reliable, and repeatable automated pipeline.

# 🛠️ Tools & Technologies Used

Apify LLM Contact Scraper – Extracts contact details from websites

N8N Automation Tool – Orchestrates the workflow and manages each step

JavaScript (inside N8N) – Cleans, formats, and structures extracted data

Google Sheets API – Stores and organizes the final cleaned data

HTTP Requests – Connects to the Apify platform using REST API

# 🔄 End-to-End Workflow Summary

Workflow Trigger
The automation starts using the "Execute Workflow" button in N8N.

Run Apify Actor
A POST request is sent to the Apify LLM Contact Scraper along with website URLs.

Wait for Actor Completion
N8N pauses until the Apify actor finishes scraping.

Fetch Dataset from Apify
A GET request retrieves the cleaned dataset from Apify’s storage.

JavaScript Data Cleaning
JS functions standardize and clean the raw fax/phone/email outputs.

Append Data to Google Sheets
Every cleaned row is automatically appended to a Google Sheet.

# 📸 Workflow Diagram

(Add your workflow diagram here)

![Workflow Diagram](images/workflow_diagram.png)

📂 Project Structure
fax-extraction-automation/
│
├── README.md
│
└── images/
    ├── workflow_diagram.png
    ├── sample_input.png
    └── sample_output.png

# ✨ Key Features

Fully Automated Contact Extraction
No manual copy-paste — complete automation from scraping to storing.

Clean & Reliable Output
JavaScript nodes remove empty values and format entries consistently.

Seamless Integrations
Apify + N8N + Google Sheets work together smoothly.

Scalable Workflow
Can handle 50 to 500+ websites easily.

# 📚 What I Learned

Integrating Apify API with automation tools

Designing clean N8N workflows for real-world use

Using JavaScript inside automation nodes for data cleanup

Handling delays, dataset IDs, and step-based execution

Creating repeatable and scalable automation pipelines

📞 Contact

Name: Azad Bhasme
