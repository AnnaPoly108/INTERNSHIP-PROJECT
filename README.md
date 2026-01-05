# INTERNSHIP-PROJECT
📚 Automated Class & Assignment Reminder System
📌 Overview

The Automated Class & Assignment Reminder System is a workflow-based automation project built using n8n. It automatically sends timely reminders to students about upcoming class sessions and assignment deadlines by reading data from Google Sheets and delivering notifications through Email and Discord.

The system eliminates manual follow-ups, ensures accurate time-based notifications (IST-aware), and improves communication efficiency in educational and training environments.

🎯 Problem Statement

Managing class schedules and assignment deadlines manually is time-consuming and error-prone, especially when handling multiple courses, batches, and students. Missed reminders can lead to absenteeism and late submissions.

This project addresses the problem by providing:

Automated schedule monitoring

Time-based notification logic

Multi-channel message delivery

Scalable and low-maintenance automation

🚀 Features

⏰ Class Session Reminders
Sends reminders when a class is about to start within a configurable time window.

📝 Assignment Deadline Alerts
Automatically notifies students when an assignment is due within the next 3 days.

📊 Centralized Data Management
Uses Google Sheets as a single source of truth for schedules and assignments.

📧 Email Notifications
Sends formal reminder emails to students.

💬 Discord Notifications
Delivers instant reminders using Discord Webhooks.

🌏 IST Timezone Handling
Accurate date and time comparison based on Indian Standard Time.

🛠️ Tech Stack

Automation Platform: n8n

Data Source: Google Sheets

Backend Logic: JavaScript (n8n Code Node)

Notification Channels:

Email (SMTP/Gmail)

Discord Webhooks

🧩 System Architecture
Google Sheets
      ↓
n8n Workflow
      ↓
Code Node (Date & Time Logic)
      ↓
 ┌───────────────┐
 │               │
Email Node     Discord Webhook

⚙️ How It Works

Google Sheets stores class schedules, assignment details, and student contact information.

n8n periodically reads data from the sheet.

A JavaScript Code Node:

Converts Excel date and time values

Compares session time with current IST

Calculates days remaining for assignments

If conditions match:

Email and Discord notifications are sent automatically.
