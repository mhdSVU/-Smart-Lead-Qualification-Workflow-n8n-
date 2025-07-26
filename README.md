# 🔁 Smart Lead Qualification Workflow (n8n)
Lead scoring &amp; Slack alerts with n8n. Auto store leads from form to Google Sheets via webhook.

This project is a real-time automation built with [n8n](https://n8n.io/) that:

- Receives leads via a webhook (e.g., Tally.so form)
- Validates and scores leads (Hot, Warm, Cold)
- Stores lead data in Google Sheets
- Sends smart Slack notifications for Hot leads
- Sends follow-up emails automatically

🧰 **Tech Stack**: n8n (self-hosted), Google Sheets, Slack (free-tier), Tally.so, SMTP

⚙️ **Features**:
- Conditional scoring logic based on `budget` and `interest_level`
- Slack alerts to sales for qualified leads
- Public Tally.so integration (no code form triggering)
- SMTP-based email follow-up with delay node
- Easily extendable for CRM or analytics integration

📌 This project showcases real-world automation use cases with clean logic, clear separation of responsibilities, and modern no-code tooling.

> 📎 No credentials are included — the workflow is fully exportable and reusable with your own API keys.

---

## 📷 Screenshots

![Workflow Overview](./docs/workflow_diagram.png)
![Slack Message](./docs/slack_message_sample.png)
![Google Sheet](./docs/google_sheet_example.png)

---

## 🚀 Getting Started

Import the included `.json` file into your n8n instance. Configure your own credentials for:

- Google Sheets API
- Slack API
- SMTP (for emails)

Test with dummy data or connect it to a live Tally.so form.

---

## 📘 Future Improvements (Optional Roadmap)

- Duplicate checking and record updates
- Integration with CRM (e.g., HubSpot, Salesforce)
- Dynamic nurture campaigns
- AI-based validation or fraud detection
