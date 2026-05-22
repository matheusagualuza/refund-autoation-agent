Gmail Refund Automation Agent
AI-powered refund request automation built with n8n, Google Gemini, and Google Sheets.
What it does
A customer fills out a refund form. The system automatically reads the request, analyzes the customer's sentiment and purchase history, classifies the customer, and routes the response — no human intervention needed.
How it works

Webhook receives form data (name, email, product, reason)
AI Agent analyzes sentiment and reads customer history from Google Sheets
Checks if purchase is within 7-day refund window
Classifies customer into three categories and acts accordingly:

Common (spent under R$3k) → automated denial email
VIP (spent over R$3k) → escalation email to customer + Telegram alert to management
Upset (negative sentiment detected) → priority escalation via email + urgent Telegram to management


Stack
n8n, Google Gemini, Google Sheets, Telegram Bot API, Webhook
