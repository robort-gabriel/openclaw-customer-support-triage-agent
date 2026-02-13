# OpenClaw Customer Support Triage Agent (Full Workspace)

AI agent that monitors support channels (email, Intercom, Zendesk, Slack, etc.), classifies incoming tickets, drafts replies, and escalates urgent issues—without auto‑sending risky responses.

## What this repo includes
- **Workspace folder** (`/workspace-customer-support-triage-agent`) containing full OpenClaw agent files
- **Workflow assets** (triage + drafting)
- **OpenClaw config template** (`openclaw.json.example`)
- **Setup guide**
- **Skills** inside the workspace

## Quick Start
1) **Clone repo**
2) Point OpenClaw to the workspace folder:
   ```json
   { "agents": { "defaults": { "workspace": "/path/to/customer-support-triage-agent/workspace-customer-support-triage-agent" } } }
   ```
3) Copy config template:
   ```bash
   cp openclaw.json.example ~/.openclaw/openclaw.json
   ```
4) Set your channel credentials in `.env` (see `.env.example`).
5) Review `workspace-customer-support-triage-agent/WORKFLOW.md`.

> Note: No auto‑sending by default. Human approval required for outbound replies.

## Output Format (Drafts)
```
[DRAFT – Approval Needed]
Category: <billing | bug | feature | onboarding | access | other>
Priority: <critical | high | medium | low>
Summary: <1–2 lines>
Suggested reply: <short draft>
Escalate: <yes/no> (reason)
```
