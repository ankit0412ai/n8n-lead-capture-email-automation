# 📩 Lead Capture & Email Automation using n8n

## Overview

This n8n workflow automates the complete lead management process by monitoring new entries in Google Sheets, validating incoming data, notifying administrators, sending confirmation emails to customers, and logging invalid submissions.

---

## Features

- 📄 Detects new leads from Google Sheets
- ✅ Validates incoming lead data
- 🔁 Processes multiple leads automatically
- 📝 Generates lead summaries
- 📧 Sends notification emails to the admin
- 📬 Sends confirmation emails to customers
- ⏳ Uses wait nodes for controlled execution
- 📊 Logs invalid entries into Google Sheets

---

## Workflow

```text
Google Sheets Trigger
        │
        ▼
   Validate Lead
      /     \
Valid       Invalid
 │             │
 ▼             ▼
Loop       Wait
 │             │
 ▼             ▼
Summarize   Append to Sheet
 │
 ▼
Email Admin
 │
 ▼
Wait
 │
 ▼
Email Customer
```

---

## Tech Stack

- n8n
- Google Sheets
- Gmail
- JavaScript Expressions

---

## Use Cases

- Contact Form Automation
- Lead Management
- CRM Automation
- Customer Acknowledgement
- Sales Notification

---

## Installation

1. Import `workflow.json` into n8n.
2. Configure Google Sheets credentials.
3. Configure Gmail credentials.
4. Update Spreadsheet IDs.
5. Activate the workflow.

---
 ## Business Value

This workflow helps businesses automate lead handling by:
- Reducing manual work
- Sending instant email notifications
- Improving customer response time
- Maintaining accurate lead records
- Eliminating repetitive administrative tasks
