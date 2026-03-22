# MisarMail Agents

Pre-built AI agent configurations for MisarMail MCP. Each agent combines multiple MCP tools into an autonomous workflow.

## Available Agents

| Agent | Tools Used | Description |
|-------|-----------|-------------|
| [Campaign Manager](campaign-manager.md) | 11 tools | Plans, creates, A/B tests, sends, and optimizes email campaigns end-to-end |
| [Deliverability Doctor](deliverability-doctor.md) | 7 tools | Monitors sender health, diagnoses DNS/reputation issues, cleans contact lists |
| [Inbox Assistant](inbox-assistant.md) | 5 tools | Reads, triages, responds to, and organizes emails across all accounts |
| [Growth Autopilot](growth-autopilot.md) | 11 tools | Manages subscriber lifecycle — acquisition, engagement, monetization, retention |
| [Multichannel Broadcaster](multichannel-broadcaster.md) | 7 tools | Coordinates email + WhatsApp + push notifications from a single prompt |

## Usage

Each agent file contains:
- **Role** — What the agent does
- **Tools Required** — Which MCP tools it needs
- **Workflow** — Step-by-step autonomous process
- **Example Prompts** — Natural language triggers
- **Configuration** — MCP server setup

Copy the agent's role description into your AI assistant's system prompt, connect to MisarMail MCP, and start prompting.

## Quick Start

```json
{
  "mcpServers": {
    "misarmail": {
      "url": "https://mail.misar.io/api/mcp",
      "transport": "http"
    }
  }
}
```

Then tell your AI: *"You are the Campaign Manager agent. Help me launch a re-engagement campaign."*
