# OpenClaw Inbox Triage Agent (Full Workspace)

An end-user-facing OpenClaw agent that classifies incoming messages, drafts safe replies, and flags anything that needs human review.

## What it does
- classifies priority
- suggests labels
- drafts replies
- recommends next actions or escalations

## What’s included
- full workspace folder
- prompt file
- triage rubric
- reply template
- smoke tests
- release checklist
- OpenClaw config template

## Quick start
1. Clone the repo.
2. Point OpenClaw to `workspace-inbox-triage-agent`.
3. Copy `openclaw.json.example` into your local OpenClaw config.
4. Fill in `.env` credentials locally.
5. Run the smoke tests.

## Output format
```
[TRIAGE – Approval Needed]
Priority: <urgent | high | normal | low>
Suggested labels: <comma-separated labels>
Summary: <1–2 lines>
Draft reply: <short draft>
Next actions: <one short line>
Escalate: <yes/no> (reason)
```

## Safety
- No auto-send.
- Human review required before outbound replies.
- Do not store secrets in the repo.
