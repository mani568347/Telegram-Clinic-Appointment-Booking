# 🏥 Telegram Clinic Appointment Booking Automation

A simple clinic appointment booking automation system built using **Telegram, n8n, Google Sheets, Docker, and Cloudflare Tunnel**.

Patients can send their appointment details directly to a Telegram bot. The n8n workflow automatically processes the message, extracts the appointment information, stores it in Google Sheets, and sends a confirmation message back to the same patient.

---

## 🚀 Features

- 📱 Telegram-based appointment booking
- ⚡ Automatic workflow execution using n8n
- 👤 Patient name extraction
- 📅 Appointment date extraction
- ⏰ Appointment time extraction
- 📝 Reason/problem extraction
- 🆔 Automatic Appointment ID generation
- 📊 Automatic Google Sheets storage
- 🤖 Automatic Telegram confirmation
- 💬 Dynamic Telegram Chat ID
- 🔄 Same-patient automatic reply
- 🐳 Self-hosted n8n using Docker
- 🔐 HTTPS webhook using Cloudflare Tunnel

---

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Telegram | Patient communication |
| n8n | Workflow automation |
| Google Sheets | Appointment data storage |
| Docker | Running n8n |
| Cloudflare Tunnel | Public HTTPS webhook |
| JavaScript | Appointment data processing |

---

## 🔄 Workflow

```text
👤 Patient
     ↓
📱 Telegram Bot
     ↓
⚡ Telegram Trigger
     ↓
🔀 Switch
     ↓
📝 Edit Fields
     ↓
💻 Code in JavaScript
     ↓
📊 Google Sheets
     ↓
🤖 Telegram Send Message
     ↓
👤 Same Patient receives confirmation
---

## 📁 Project Files

```text
Telegram-Clinic-Appointment-Booking/
│
├── README.md
├── .gitignore
└── telegram-clinic-appointment-workflow-safe.json
