# P1: Review Responder (n8n Automation)

## Overview
An automated workflow built with n8n to monitor incoming Google reviews, draft AI responses using the free-tier Gemini API, and submit them to Slack for human approval.

## Architecture
1. **Webhook Trigger**: Receives Google Review payload (`customer_name`, `rating`, `review_text`).
2. **AI Processing**: Google Gemini API drafts a polite, tailored response.
3. **Approval Notification**: Sends formatted review & draft reply to Slack `#reviews-approval` channel.

## Local Setup
1. Import `workflow.json` into your local n8n instance.
2. Set up environment variables based on `.env.example`.

## Tools Used
- n8n (Community Edition)
- Google Gemini API (Free Tier)
- Slack Webhook Integration