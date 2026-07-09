# Workshop Admin Agent for Slack

> An AI-powered Slack agent that helps workshop administrators manage workshops, registrations, attendance, and performance—without leaving Slack.

---

# Overview

Workshop Admin Agent for Slack brings workshop management directly into Slack by combining conversational AI with Salesforce. Instead of switching between multiple administrative tools, workshop organizers can manage the entire workshop lifecycle using natural language.

The agent acts as an intelligent assistant that understands administrator requests and securely performs the corresponding Salesforce operations.

---

# Inspiration

Workshop administrators often spend a significant amount of time switching between communication platforms and learning management systems to handle registrations, attendance tracking, scheduling, reporting, and participant engagement.

Since many organizations already collaborate in Slack, we wanted to make workshop administration as simple as having a conversation. Our goal was to reduce repetitive administrative work and allow organizers to focus on delivering better learning experiences.

---

# What It Does

The Workshop Admin Agent enables administrators to manage workshops entirely from Slack.

### Workshop Management

- Create new workshops
- Update workshop information
- Publish or cancel workshops
- Manage workshop schedules

**Screenshot**

> 📷 _Placeholder: Workshop creation in Slack_

![Workshop Creation](docs/images/workshop-creation.png)

---

### Registration Management

- View registrations
- Manage waiting lists
- Approve or remove participants

**Screenshot**

> 📷 _Placeholder: Registration management_

![Registration Management](docs/images/registrations.png)

---

### Attendance & Engagement

- Track attendance
- Monitor participant engagement
- View completion statistics

**Screenshot**

> 📷 _Placeholder: Attendance dashboard_

![Attendance Dashboard](docs/images/attendance-dashboard.png)

---

### Notifications

Administrators can configure reminders and notifications for upcoming workshops, registration deadlines, and participant updates.

**Screenshot**

> 📷 _Placeholder: Reminder configuration_

![Notifications](docs/images/notifications.png)

---

### Analytics & Reporting

The agent provides dashboards and natural language reporting, allowing administrators to quickly understand workshop performance.

Example prompts:

> "Show workshops scheduled for this month."

> "Create a new AI Fundamentals workshop for next Friday."

> "Which workshops had the highest attendance rate?"

**Screenshot**

> 📷 _Placeholder: Analytics dashboard_

![Analytics](docs/images/analytics-dashboard.png)

---

# Architecture

The solution combines several Salesforce and Slack technologies:

- Slack AI Agent
- Salesforce Platform
- Custom Salesforce Objects
  - Workshops
  - Attendees
  - Instructors
  - Reviews
- Natural language interaction through Slack

Salesforce serves as the system of record while Slack provides the conversational interface for administrators.

```text
+------------------+
|      Slack       |
|   AI Agent UI    |
+--------+---------+
         |
         v
+------------------+
|  AI Agent Logic  |
+--------+---------+
         |
         v
+------------------+
|   Salesforce     |
|------------------|
| Workshops        |
| Registrations    |
| Attendance       |
| Reviews          |
+------------------+
```

---

# Challenges

One of the biggest challenges was designing an experience that feels conversational while supporting complex administrative workflows.

Additional challenges included:

- Designing intuitive conversational flows
- Mapping natural language to Salesforce operations
- Maintaining permission-aware responses
- Presenting administrative data clearly within Slack
- Supporting multiple workshop management scenarios through a chat interface

---

# What We Learned

This project demonstrated how conversational AI can significantly simplify operational workflows.

Some key takeaways include:

- Natural language is an effective interface for administrative tasks.
- Slack can become more than a messaging platform—it can serve as a productivity workspace.
- Salesforce provides a robust backend for AI-driven business applications.
- Permission-aware AI interactions are essential for enterprise environments.

---

# Future Improvements

Potential future enhancements include:

- Calendar integration (Google Calendar / Outlook)
- AI-generated workshop summaries
- Attendance prediction
- Automated follow-up messages
- Participant feedback analysis
- Multi-language support

---

# Tech Stack

- Slack
- Salesforce
- Salesforce AI
- Apex
- Custom Salesforce Objects
- Natural Language Processing

---

# Demo

**Screenshot**

> 📷 _Placeholder: Complete workflow demo_

![Demo](docs/images/demo.png)

---

# Repository Structure

```
docs/
└── images/
    ├── analytics-dashboard.png
    ├── attendance-dashboard.png
    ├── demo.png
    ├── notifications.png
    ├── registrations.png
    └── workshop-creation.png
```

---

# Elevator Pitch

> **An AI-powered Slack agent that helps workshop administrators manage workshops, registrations, attendance, and performance without leaving Slack.**
