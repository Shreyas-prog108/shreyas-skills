# Project Planning Template

Use this file to give AI coding tools the context they need before design or implementation work starts. Update it at the beginning of a project and whenever major decisions change.

## Goal

What are we building, and what user problem does it solve?

## Users

Who uses this, and what outcome do they care about?

## Scope

What is included in the current version?

## Non-Goals

What should not be built right now?

## Architecture Notes

Key technical choices, constraints, services, frameworks, data stores, and external APIs.

## Agent Design

If this project uses agents, define:

- Perceive: what inputs, tools, memory, and context the agent receives.
- Reason: what decisions the agent makes.
- Act: what tools, APIs, writes, or messages the agent produces.
- Observe: how success or failure is detected.
- Terminate: when the workflow ends or escalates.

## Failure Modes

List the top three things likely to break and how the implementation should handle them.

## Environment Variables

Use placeholder names only. Do not include real secrets.

```env
API_KEY=your_api_key_here
DATABASE_URL=your_database_url_here
```

## Definition Of Done

- The core workflow works for the happy path.
- The main failure modes are handled.
- Tests exist for important logic.
- No real `.env`, `.env.local`, `.env.*.local`, API key, or secret is read, printed, or committed.
- The implementation follows `coding-skills.md`.
