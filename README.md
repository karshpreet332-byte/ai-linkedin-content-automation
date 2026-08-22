
# AI-Powered LinkedIn Content Automation

An AI-powered LinkedIn content automation workflow built using **n8n**, **OpenAI**, and **Google Sheets**. The workflow automates the process of retrieving content, filtering records, generating LinkedIn-ready content using an AI Agent, and updating the processed records.

## Overview

This project demonstrates an end-to-end workflow automation pipeline that combines **workflow automation, AI-powered content generation, structured data processing, and LinkedIn integration**.

The workflow is designed to reduce repetitive manual work involved in preparing and publishing LinkedIn content.

## Workflow

```text
Google Sheets
      ↓
Conditional Filtering
      ↓
Limit
      ↓
AI Agent
      ↓
OpenAI Chat Model
      ↓
Structured Output Parser
      ↓
LinkedIn
      ↓
Google Sheets
```

## Key Features

* Retrieves content/data from **Google Sheets**
* Uses conditional logic to filter relevant records
* Controls the number of records processed using a limit
* Generates content using an **AI Agent and OpenAI**
* Uses a **Structured Output Parser** for consistent output
* Automates LinkedIn content creation/posting
* Updates processed records in Google Sheets
* Reduces repetitive manual content-processing tasks

## Technologies Used

* **n8n** – Workflow automation
* **OpenAI** – AI-powered content generation
* **Google Sheets** – Data storage and workflow tracking
* **LinkedIn** – Content publishing
* **AI Agent** – Content generation and processing
* **Structured Output Parser** – Structured AI output

## How It Works

1. The workflow retrieves input data from Google Sheets.
2. An **IF condition** checks and filters the relevant records.
3. A **Limit** node controls how many records are processed.
4. The selected content is passed to an **AI Agent**.
5. The AI Agent uses the **OpenAI Chat Model** to generate the required content.
6. The **Structured Output Parser** formats the generated response into a consistent structure.
7. The processed content is sent to **LinkedIn**.
8. The corresponding Google Sheets records are updated to track the processed content.

## Project Structure

```text
ai-linkedin-content-automation/
│
├── workflow/
│   └── linkedin-automation.json
│
├── screenshots/
│   ├── workflow.png
│   └── linkedin-post.png
│
├── sample-data/
│   └── sample-google-sheet.csv
│
├── .gitignore
└── README.md
```

## Screenshots

### n8n Workflow

![n8n Workflow](screenshots/workflow.png)

### LinkedIn Output

![LinkedIn Output](screenshots/linkedin-post.png)

## Setup

1. Install or access an **n8n** instance.
2. Import the workflow JSON file from the `workflow` folder.
3. Configure the required Google Sheets, OpenAI, and LinkedIn credentials in n8n.
4. Connect the workflow to the required Google Sheet.
5. Update the workflow configuration according to your data structure.
6. Execute the workflow and verify the generated LinkedIn content.

## Security

Credentials, API keys, access tokens, passwords, and other sensitive information are **not included in this repository**.

Configure credentials securely through n8n's credential management system before running the workflow.

## Learning Outcomes

This project provided hands-on experience with:

* Workflow automation using n8n
* AI Agent and OpenAI integration
* Conditional workflow logic
* Structured data processing
* API/service integration
* Automated content generation
* Google Sheets-based data management
* End-to-end automation design
