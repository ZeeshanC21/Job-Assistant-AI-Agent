# Job-Assistant-AI-Agent

This project is a fully automated Job Application Assistant built using **n8n**, OpenAI, DeepSeek, Google Sheets, Gmail, and Perplexity AI. It helps job-seeking students and professionals streamline their job application process by automatically discovering job listings, customizing cover letters, and sending applications — all without manual intervention.

---

-  Features

*End-to-End Automation**-: From job scraping to resume submission.
*RSS + LinkedIn Feed Parsing*: Automatically fetches new job listings using LinkedIn and RSS feeds.
*AI-Powered Email Generator*: Uses OpenAI to draft personalized cover letters based on job descriptions.
*Perplexity + DeepSeek API Integration*: Extracts recruiter contact info and generates accurate summaries.
*Auto Email Sending via Gmail*: Sends out tailored applications with resumes attached.
*Google Sheets Tracking*: Logs all applied jobs and statuses for future reference.
*Attachment Support*: Attaches your resume from Google Drive automatically.

---

- Tech Stack

| Tool            | Purpose                                        |
|-----------------|------------------------------------------------|
| n8n             | Core workflow automation                       |
| Google Sheets   | Tracking previous and new job applications     |
| RSS Feed        | Pulls job listings from specified sources      |
| OpenAI (GPT-4)  | Generates personalized cover letters           |
| Perplexity API  | Retrieves recruiter emails & contact details   |
| DeepSeek API    | Summarizes job descriptions                    |
| Gmail API       | Sends email applications                       |
| Google Drive    | Stores and attaches the resume (PDF)           |

---

- Workflow Overview

1. *Trigger*: Manual or scheduled trigger starts the workflow.
2. *Read Existing Applications*: Fetches previously applied jobs from Google Sheets.
3. *Scrape New Jobs*: Uses RSS to gather fresh listings.
4. *Summarize + Extract Contact Info*: Uses DeepSeek and Perplexity to summarize job descriptions and pull recruiter emails.
5. *Generate Email Content*: OpenAI generates a customized HTML cover letter.
6. *Send Email*: Gmail node sends the resume + cover letter to the hiring manager.
7. *Update Google Sheet*: Logs the new application to avoid duplicates.

---

- Setup Instructions

> You must self-host or use an n8n cloud instance to run this project.

1. Clone the Repo and get the JSON
1.git clone https://github.com/yourusername/job-assistant-automation.git
2.Set up Credentials
3.OpenAI API Key
4.Perplexity API Key
5.DeepSeek API Key
6.Gmail credentials (OAuth2 recommended)
7.Google Sheet credentials

8.Import Workflow
9.Open n8n
10.Click “Import Workflow” and upload the JSON
11.Connect Nodes
12.Authenticate all APIs
13.Update Google Sheet ID and Gmail address
14.Customize Resume
15.Upload your PDF resume to Google Drive
16.Set the download URL in the Google Drive node

- To-Do
Add fallback email templates
Integrate LinkedIn Easy Apply API
Add dashboard for tracking results
Improve error handling & alerts

- Why This Project Matters
This automation solves a real problem for job-seeking students — saving them countless hours by eliminating the repetitive, manual steps of applying to jobs. It's especially useful for batch applications while maintaining personalization — a critical factor in application success.

- Demo
Coming soon – video walkthrough & screenshots

Author
Zeeshan Charolia
📧 charoliazeeshan@gmail.com
🌐 LinkedIn
