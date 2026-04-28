# Ultimate-Watersports-ai-agent
Ultimate Watersports Operations AI Agent — Weather monitoring, booking management, and automated safety alerts across 5 locations.

ultimate-watersports-ai-agent/
├── workflows/
│   └── wf-agent-01.json          ← Put your exported workflow here
├── README.md
├── .env.example
└── LICENSE

# Ultimate Watersports Operations AI Agent

An intelligent n8n AI agent that helps manage daily operations for Ultimate Watersports across 5 locations.

## Features

- Checks weather conditions for all 5 locations (Hillarys Boat Harbour, South Perth, Geraldton, Exmouth, Broome)
- Retrieves today's bookings from FareHarbor
- Automatically identifies customers who need weather alerts
- Logs all actions to Google Sheets
- Sends test alert emails when dangerous weather is detected

## Tech Stack

- **n8n** + LangChain
- **Groq** (Llama 3.3 70B / 8B models)
- Google Sheets (logging)
- Custom JavaScript tools

## How to Use

1. Import `workflows/wf-agent-01.json` into n8n
2. Set up credentials:
   - Groq API Key
   - Google Sheets OAuth2
3. Configure the tools (especially `send_customer_email`)
4. Trigger via Chat Trigger

## Current Status

**Stable Working Version** - Basic weather checking, booking retrieval, logging, and test email functionality are working.

Future improvements planned:
- Real FareHarbor API integration
- Better alerting logic
- Equipment status integration

---

Made for Ultimate Watersports Operations Team
