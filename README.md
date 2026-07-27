# 🤖 AI Lead Qualification Assistant

## 📌 Project Overview

The AI Lead Qualification Assistant is an automation workflow built using **n8n** that analyses incoming customer enquiries, extracts lead information using **Google Gemini AI**, qualifies the lead based on predefined business rules, stores qualified leads in **Google Sheets**, schedules a follow-up event in **Google Calendar**, and sends email notifications through **Gmail**.

The workflow reduces manual effort in lead management by automatically identifying high-quality business opportunities.

---

## 🚀 Features

- AI-powered lead information extraction
- Automatic lead qualification
- Lead scoring (0–100)
- Priority assignment (High / Medium / Low)
- Google Sheets integration
- Google Calendar event creation
- Gmail notifications
- Human handoff for non-qualified leads
- Multi-language prompt support (implemented)

---

## 🛠 Technologies Used

- n8n
- Google Gemini AI
- Google Sheets
- Google Calendar
- Gmail
- JavaScript
- Postman

---

## 📊 Workflow Architecture

```
Webhook
      │
      ▼
Google Gemini AI
      │
      ▼
JavaScript (Parse JSON)
      │
      ▼
IF (Qualified?)
      ├───────────────┐
      │               │
      ▼               ▼
Google Sheets      Manual Review Email
      │
      ▼
Google Calendar
      │
      ▼
Qualified Lead Email
```

---

## 📋 Lead Qualification Rules

A lead is marked as **Qualified** if at least **two** of the following conditions are satisfied:

- Budget ≥ ₹1,00,000
- Timeline ≤ 6 months
- Requirement related to:
  - AI
  - Automation
  - Software Development
  - Chatbots
  - Web Applications
  - Mobile Applications

The AI also generates:

- Lead Score
- Priority
- Qualification Reason

---

## 📂 Project Structure

```
AI-Lead-Qualification-Assistant
│
├── AI Lead Qualification Assistant.json
├── README.md
└── screenshots/
```

---

## ⚙️ Setup Instructions

1. Import the workflow JSON into n8n.
2. Configure Google Gemini API credentials.
3. Connect Google Sheets.
4. Connect Gmail.
5. Connect Google Calendar.
6. Activate the workflow.
7. Test using Postman.

---

## 🧪 Example Test

### Input

```json
{
  "message":"Hello, I'm Aarav Menon from IntelliCore Solutions. We need an AI-powered workflow automation system with a budget of ₹12,00,000 to be completed within 5 months."
}
```

### Expected Output

- Qualified Lead
- Lead Score: 95
- Priority: High
- Google Sheet Updated
- Calendar Event Created
- Email Notification Sent

---

## 📸 Screenshots

(Add workflow, Gmail, Google Sheets, Calendar and Postman screenshots here.)

---

## 🔮 Future Enhancements

- CRM Integration
- Slack / Microsoft Teams Notifications
- Voice Input Support
- Dashboard & Analytics
- Database Integration
- AI Memory
- Advanced Multi-language Support

---

## 👩‍💻 Author

**Mamidi Pavani**

AI & Automation Engineer Intern Assignment
