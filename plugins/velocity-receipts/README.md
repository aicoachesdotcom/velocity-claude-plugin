# Velocity · Claude Code plugin

Records every Velocity skill invocation in Claude Code and reports it
back to your [Velocity](https://velocity.forum) account, so
Value Impact (V.I.) compounds across your real work — not just inside
facilitated CoWork sessions.

## Install

```
claude plugin marketplace add aicoachesdotcom/velocity-claude-plugin
claude plugin install velocity-receipts@aicoaches
```

On first enable you'll be prompted for a **Velocity install code**
(optional — from your Velocity Desktop session-complete screen; leave
blank to authorize via the browser device-code flow) and a **server
URL** (defaults to the AiCoaches-hosted tenant).

## What it does

- Holds a scoped Velocity API token in
  `~/.claude/plugins/velocity-receipts/config.json`.
- Syncs your per-activity `SKILL.md` files into
  `~/.claude/skills/velocity-*/` and keeps them current.
- Records each skill invocation + flushes V.I. receipts back to
  Velocity (batched, retried, idempotent).

## Tools

`record_invocation`, `complete_invocation`, `status`,
`pause_telemetry`, `resume_telemetry`.

## Privacy

Telemetry is opt-out anytime (`pause_telemetry`) and revocable from
Velocity → Settings → Skills · MCP. The server reads only the scopes
you approve. Full privacy policy: https://velocity.forum/privacy — see
LICENSE for terms.

---

© AiCoaches.com LLC. Built for [Velocity](https://velocity.forum).
