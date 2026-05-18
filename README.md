# Auto Email Replier 🤖📬

An n8n automation workflow that reads incoming Gmail messages, classifies urgency using Google Gemini AI, drafts a professional reply, and notifies you on Telegram.

## Workflow
Gmail Trigger → Gemini AI → Parse Response → Create Gmail Draft + Telegram Alert

## Features
- Classifies emails as High / Medium / Low urgency
- Auto-drafts replies using Gemini 1.5 Flash
- Stars high-urgency emails automatically
- Sends a Telegram notification with urgency summary
- Draft goes to Gmail for review before sending — you're always in control

## Setup
1. Import `ai_email_reply_generator.json` into your n8n instance
2. Add credentials:
   - Gmail OAuth2
   - Gemini API key (Google AI Studio)
   - Telegram Bot token + Chat ID
3. Activate the workflow

## Tech Stack
- [n8n](https://n8n.io) — workflow automation
- Google Gemini 1.5 Flash — email classification & reply drafting
- Gmail API — trigger + draft creation
- Telegram Bot API — notifications
