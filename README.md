# n8n Webhook → Gmail Automation

This project demonstrates a basic automation workflow using **n8n**, where an incoming webhook request triggers an email to be sent via Gmail.

---

## What I Implemented

* Created a **Webhook node** in n8n to receive HTTP POST requests
* Configured a **Gmail node** to send emails dynamically
* Connected webhook data (JSON) to email fields

---

## Workflow

Webhook Request → n8n → Gmail (Email Sent)

---

## How It Works

1. A POST request is sent to the n8n webhook
2. The webhook captures incoming JSON data
3. Data is passed to the Gmail node
4. Email is sent using provided details

---

## Sample Request

```id="req1"
POST /webhook/send-email
Content-Type: application/json

{
  "to": "your-email@example.com",
  "subject": "Test Email",
  "message": "This is sent via n8n webhook"
}
```

---

## Output

* n8n execution shows successful workflow run
* Email received in Gmail inbox

---

## Key Learning

* Understanding webhook-based triggers
* Integrating external HTTP requests with automation workflows
* Using n8n nodes for real-time processing

---

## License

MIT
