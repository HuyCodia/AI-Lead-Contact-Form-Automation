# AI Lead & Contact Form Automation

An AI-powered contact management workflow built with **n8n**, integrating **Google Gemini**, **Gmail** and **Google Sheets** to automatically analyze, categorize and route incoming business inquiries.

## Overview

This project automates the processing of incoming contact form submissions using AI and workflow automation.

Google Gemini analyzes each inquiry, determines its category, priority and sentiment, generates a concise summary and recommends the next appropriate action.

Based on the AI analysis, inquiries are automatically routed to the relevant department, while submission data and notification details are stored in Google Sheets.

## Features

- **Contact Form Integration** – Collect incoming inquiries, including contact details, subject and message.
- **AI-powered Analysis** – Analyze submissions using Google Gemini.
- **Automatic Categorization** – Classify inquiries into Sales, Support, Application or Other.
- **Priority Assessment** – Assign Low, Medium or High priority levels.
- **Sentiment Analysis** – Identify the sentiment of incoming inquiries.
- **AI-generated Summaries** – Generate concise summaries and recommended next steps.
- **Automatic Department Routing** – Forward inquiries to the appropriate department.
- **Email Notifications** – Generate and send department-specific HTML email notifications.
- **Google Sheets Integration** – Store original submissions, AI analysis results and notification details.

## Technologies

- n8n
- Google Gemini (`gemini-2.5-flash`)
- Gmail
- Google Sheets
- JavaScript
- HTML
- JSON

## Workflow

1. A user submits an inquiry through the contact form.
2. n8n receives the form submission.
3. Google Gemini analyzes the submitted information.
4. The AI generates a structured response containing category, priority, sentiment, summary and recommended next step.
5. The original form data is merged with the AI analysis.
6. The inquiry is stored in Google Sheets.
7. Based on its category, the inquiry is routed to the appropriate department.
8. A department-specific HTML email notification is generated and sent.
9. Notification details are stored in a second Google Sheets tab.

## Project Structure

```text
ai-lead-contact-form-automation/
├── screenshots/
│   └── workflow-overview.png
├── workflow/
│   └── Al-Lead-&-Contact-Form-Automation.json
└── README.md
```

## Setup

1. Import the workflow JSON file into your n8n instance.
2. Configure your Google Gemini credentials.
3. Connect your Gmail account.
4. Connect your Google Sheets account.
5. Create a Google Spreadsheet with the required columns and two worksheet tabs.
6. Replace the spreadsheet ID placeholder and configure the corresponding worksheet tabs.
7. Set the appropriate recipient email addresses for each department.
8. Test the workflow with sample submissions before activating it.

**Note:** API credentials, OAuth tokens and personal customer data are not included in this repository. You must configure your own credentials and integrations before running the workflow.

## Purpose

This project demonstrates practical experience with AI-powered workflow automation, structured LLM output, automated data processing and integrations between external services using n8n.