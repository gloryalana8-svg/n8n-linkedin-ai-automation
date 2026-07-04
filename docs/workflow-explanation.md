# Workflow Documentation

## Project Overview

This project automates the creation and publishing of LinkedIn posts using n8n and Google Gemini AI.

The workflow detects new content ideas added to a Google Sheet, generates a professional LinkedIn post using AI, publishes it automatically, and updates the spreadsheet to indicate that the post has been published.

---

## Workflow Architecture

Google Sheets Trigger
↓
Code (JavaScript)
↓
AI Agent (Google Gemini)
↓
LinkedIn Create Post
↓
Google Sheets Update Row

---

## Node Explanation

### 1. Google Sheets Trigger

- Watches a Google Sheet for newly added rows.
- Starts the workflow automatically when new content is added.

### 2. Code Node

- Processes the data from Google Sheets.
- Formats the content before sending it to the AI Agent.

### 3. AI Agent (Google Gemini)

- Receives the processed content.
- Generates a professional LinkedIn post using AI.

### 4. LinkedIn Node

- Publishes the AI-generated post to LinkedIn.

### 5. Google Sheets Update Row

- Updates the processed row.
- Marks the post as "Published" to prevent duplicate posts.

---

## Technologies Used

- n8n
- Google Sheets API
- Google Gemini API
- LinkedIn API
- JavaScript

---

## Learning Outcomes

This project helped me learn:

- Workflow Automation
- AI Integration
- API Authentication
- Google Sheets Automation
- Prompt Engineering
- Business Process Automation
- AI-Powered Content Generation

---

## Future Improvements

- Schedule posts automatically.
- Generate images using AI.
- Add error notifications via email or Slack.
- Store analytics for published posts.
- Support multiple social media platforms.
