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

### 1. Clone the Repository
git clone https://github.com/yourusername/job-assistant-automation.git

2. Set Up Credentials
Make sure the following credentials are available:

🔑 OpenAI API Key

🔑 Perplexity API Key

🔑 DeepSeek API Key

🔑 Gmail credentials (OAuth2 recommended)

🔑 Google Sheets credentials

3. Import the Workflow
Open your n8n instance

Click "Import Workflow"

Upload the provided JSON file

4. Configure Nodes
Authenticate all API nodes

Update the Google Sheet ID

Update the Gmail sender address

5. Customize Resume
Upload your PDF resume to Google Drive

In the Google Drive node, set the download URL

- To-Do
 Add fallback email templates

 Integrate LinkedIn Easy Apply API

 Add dashboard for tracking results

 Improve error handling & alerts

Why This Project Matters: 

This automation solves a real problem for job-seeking students — eliminating repetitive and manual steps in applying to jobs. It’s especially useful for sending batch applications while still maintaining the personalization that helps applicants stand out.

Demo:

Coming soon – video walkthrough & screenshots

Author:

Zeeshan Charolia
- charoliazeeshan@gmail.com
- [LinkedIn](https://www.linkedin.com/in/zeeshancharolia)
