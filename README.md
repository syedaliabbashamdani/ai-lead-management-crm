<p align="center">
  <img src="workflow-images/banner%20(2).png" alt="AI Lead Management CRM Banner">
</p>

# 📘 N8N Lead Management CRM

## 🎯 Project Overview

I developed an automated Lead Management CRM using n8n, Airtable, and Slack.

The system receives customer information through a website form, processes incoming lead data, checks existing CRM records, manages lead information, assigns priorities, and sends notifications to the sales team.

The main objective is to help businesses manage incoming leads efficiently without relying on repetitive manual work.

---
## 📚 Project Documentation

For a detailed explanation of the workflow architecture, individual nodes, configuration, and business applications, read the complete project walkthrough:

📖 **[Read the Complete Project Walkthrough](docs/PROJECT-WALKTHROUGH.md)**

---

## ⚠️ Business Problem

Businesses often receive leads through website forms and manually enter customer information into spreadsheets or CRM systems.

This process can create several challenges:

- Delayed responses to potential customers.
- Repetitive manual data entry.
- Poor lead organization.
- Duplicate customer records.
- Difficulty identifying high-priority leads.
- Missed business opportunities.

---

## 💡 Solution

I developed an n8n automation workflow that connects a website lead form with Airtable CRM and Slack.

The automation handles:

- Incoming lead collection.
- Customer data processing.
- Duplicate lead checking.
- Lead scoring and priority classification.
- CRM record creation and updating.
- Priority-based Slack notifications.

---

## 🏗️ Workflow Architecture


The system follows this architecture:

```mermaid
flowchart TD
    A["🌐 Website Lead Form<br/>Customer Submits Information"]
    B["⚙️ n8n Webhook<br/>Receives Lead Information"]
    C["🤖 Data Processing & Lead Classification<br/>Organizes Data & Assigns Priority"]
    D["🗄️ Airtable CRM<br/>Store & Manage Lead Records"]
    E["💬 Slack Notifications<br/>Notify Sales Team"]

    A --> B
    B --> C
    C --> D
    D --> E

    F["🔗 n8n Automation"] -.-> B
    G["🧠 AI Processing"] -.-> C
    H["📊 CRM Integration"] -.-> D
    I["📨 Team Communication"] -.-> E

    style A fill:#E1F5FE,stroke:#0288D1,stroke-width:2px,color:#01579B
    style B fill:#E8EAF6,stroke:#3949AB,stroke-width:2px,color:#1A237E
    style C fill:#F3E5F5,stroke:#8E24AA,stroke-width:2px,color:#4A148C
    style D fill:#E8F5E9,stroke:#43A047,stroke-width:2px,color:#1B5E20
    style E fill:#E0F2F1,stroke:#00897B,stroke-width:2px,color:#004D40
    style F fill:#ECEFF1,stroke:#546E7A,stroke-width:2px,color:#263238
    style G fill:#FCE4EC,stroke:#D81B60,stroke-width:2px,color:#880E4F
    style H fill:#FFF9C4,stroke:#F9A825,stroke-width:2px,color:#795548
    style I fill:#FFF3E0,stroke:#FB8C00,stroke-width:2px,color:#E65100
```

---

## ⚙️ Workflow Process

The automation is divided into two main stages.

### Stage 1: Lead Capture & Database Management

1. **Webhook:** Receives incoming customer information from the website lead form.
2. **Edit Fields:** Organizes and prepares the incoming lead data.
3. **IF Node:** Evaluates the lead-processing condition.
4. **Airtable Search Records:** Checks whether the lead already exists in the CRM.
5. **IF Node:** Determines how to handle new and existing records.
6. **Airtable Create Record:** Stores new lead information in Airtable.

### Stage 2: Lead Scoring & Notifications

1. **Lead Scoring:** Processes lead information and assigns a priority.
2. **Airtable Update Record:** Updates the CRM record with the scoring information.
3. **Check Lead Priority:** Evaluates the assigned lead priority.
4. **High Priority Notification:** Sends a dedicated Slack notification for high-priority leads.
5. **Standard Notification:** Sends a standard Slack notification for normal-priority leads.

---

## ✨ Key Features

- 🌐 Automated website lead capture.
- 📝 Customer information processing.
- 🔍 Duplicate lead detection.
- 📊 Automated lead scoring.
- 🚦 Lead priority classification.
- 🗄️ Airtable CRM integration.
- 💬 Slack team notifications.
- ⚡ Reduced manual data entry.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| n8n | Workflow automation |
| Airtable | Lead database and CRM |
| Slack | Sales team notifications |
| Webhooks | Incoming lead collection |
| JSON | Structured data processing |

---

## 📸 Workflow Screenshots

### 1. Complete n8n Workflow

The complete Lead Management CRM automation, showing the connected workflow stages.

![Complete n8n Lead Management Workflow](workflow-images/Screenshot%202026-11-08%20134343.jpg)

### 2. Successful Workflow Execution

Demonstration of successful lead capture and processing.

![Successful Workflow Execution](workflow-images/image%20(11).png)

### 3. Webhook Incoming Data

Incoming customer information received through the n8n Webhook node.

![Webhook Incoming Data](workflow-images/image%20(12).png)

### 4. Airtable CRM Record

Customer lead information successfully stored in Airtable.

![Airtable CRM Record](workflow-images/image%20(13).png)

### 5. Slack Notification

Lead notification successfully delivered to the Slack team.

![Slack Notification](workflow-images/image%20(14).png)

---

## 📊 Results

The workflow was successfully tested and demonstrated the following:

- Incoming test leads were received through the webhook.
- Customer information was processed.
- Lead records were stored in Airtable.
- Lead priority was evaluated.
- Slack notifications were sent according to lead priority.

The project demonstrates an automated process for managing incoming business leads.

---

## 💼 Business Benefits

This automation can help businesses:

- Reduce repetitive manual data entry.
- Keep customer information organized.
- Identify important leads more efficiently.
- Improve sales team visibility.
- Reduce the risk of missed leads.
- Centralize lead information in Airtable.

---


## 📌 Project Information

| Detail | Description |
|---|---|
| Project Name | AI Lead Management CRM |
| Project Type | Personal Automation Project |
| Automation Platform | n8n |
| CRM Database | Airtable |
| Notification Platform | Slack |
| Project Status | Completed |
| Demonstration | Test workflow execution |

---

## 🚀 Need a Similar Automation?

I can help businesses build custom automation systems for:

- Lead capture and management.
- CRM automation.
- Automated lead qualification.
- Sales team notifications.
- Business process automation.
- API and application integrations.

**Let's automate your business processes!**

👨‍💻 **Developer:** Syed Ali Abbas

🔗 **GitHub:** [github.com/syedaliabbashamdani](https://github.com/syedaliabbashamdani)

