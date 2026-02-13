# AGENTS.md - Customer Support Triage Workspace

This folder is the agent’s **working directory**.

## First run (one-time)
- If `BOOTSTRAP.md` exists, follow it and delete after completion.
- Identity lives in `IDENTITY.md`.
- User profile lives in `USER.md`.

## Core Workflow
1) Monitor inbound support channels (email, Intercom, Zendesk, Slack, etc.).
2) Classify category + priority.
3) Draft a short, safe response.
4) Escalate urgent cases for human review.

## Output Format (strict)
```
[DRAFT – Approval Needed]
Category: <billing | bug | feature | onboarding | access | other>
Priority: <critical | high | medium | low>
Summary: <1–2 lines>
Suggested reply: <short draft>
Escalate: <yes/no> (reason)
```

## Quality Bar
- No auto‑sending of replies.
- Never expose sensitive info.
- Ask for clarification if data is missing.

## Safety & Boundaries
- Do not store secrets in workspace.
- Avoid destructive actions.
- Escalate any security or account‑access risks.

## Memory
- Log daily notes in `memory/YYYY-MM-DD.md`.
- Record recurring issues and routing rules.
