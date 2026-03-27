# 📢 Serverless Event Announcement System

A modern, responsive web application that allows users to broadcast event announcements. This project leverages a fully serverless AWS architecture to handle data processing and real-time notifications.

## 🏗️ Architecture Overview

The system follows a decoupled, serverless workflow:
1.  **Frontend:** Hosted on **AWS S3** (Static Website Hosting).
2.  **API Layer:** **AWS API Gateway** receives REST requests from the frontend.
3.  **Compute:** **AWS Lambda** (Python/Node.js) processes the announcement logic.
4.  **Notification:** **AWS SNS** (Simple Notification Service) sends emails/SMS to subscribers instantly.
gg


---

## 📁 Project Structure

```text
.
├── frontend/
│   ├── index.html        # Modern Glassmorphism UI
│   ├── style.css         # Custom CSS with animations
│   └── script.js         # API Integration (Fetch/Axios)
├── backend/
│   └── lambda_function.py # AWS Lambda logic to trigger SNS
├── terraform/            # (Optional) IaC for infrastructure
└── README.md
