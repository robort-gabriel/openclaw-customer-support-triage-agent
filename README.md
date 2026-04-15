# OpenClaw Inbox Triage Agent

Production-ready draft package for an end-user inbox triage assistant.

## Install
1. Clone the repo.
2. Copy `openclaw.json.example` into your local OpenClaw config.
3. Point the agent workspace at `workspace-inbox-triage-agent`.
4. Fill in channel credentials in `.env`.
5. Run the smoke tests in `workspace-inbox-triage-agent/SMOKE_TESTS.md`.

## Included
- triage workspace
- prompt file
- rubric
- reply template
- smoke tests
- release checklist
- package overview

## Safety
- No auto-send.
- Human review before outbound replies.
- Keep secrets out of the repo.
