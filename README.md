# 👋 Welcome to OdooDevTools Discussions

This is the community space for **OdooDevTools** — a SaaS platform that gives Odoo developers real-time visibility into performance, queries, ACL issues, and schema changes across their environments.

If you've ever spent hours staring at SQL logs trying to track down a slow endpoint, this is built for you.

---

## What is OdooDevTools?

OdooDevTools is a lightweight agent + cloud dashboard that connects to your Odoo instance and surfaces what's actually happening under the hood — without you having to piece it together manually.

**Core features:**

- 🔍 **N+1 Detection** — automatically flags repeated ORM patterns with fix suggestions
- 📊 **Waterfall Profiler** — see a full timeline of ORM and SQL calls for a single request
- 🔐 **ACL Debugger** — trace exactly why an access error is being thrown (user → groups → model rules → record rules → domain)
- 🗄️ **Schema Tracker** — snapshot your Odoo schema and diff it across environments or versions
- 🚨 **Performance Budgets** — set thresholds per endpoint and get alerted when they're breached
- 🔄 **Migration Scanner** — scan your codebase for breaking changes before upgrading Odoo versions
- 🧹 **Anonymizer** — detect and anonymize PII fields for safe staging environments

**How it works:**

A single Go binary (the agent) runs on your Odoo server. It samples ORM calls, aggregates data locally, and streams it to the cloud dashboard over a persistent WebSocket. No Python environment needed — just drop in the binary and run it.

---

## Discussion Categories

Use the tabs above to find the right place for your topic:

| Category | What to post |
|---|---|
| 💡 **Ideas** | Feature requests, workflow improvements, things you wish existed |
| 🐛 **Bug Reports** | Something not working as expected — include your Odoo version and agent version |
| 🙋 **Q&A** | Questions about setup, usage, or how a feature works |
| 🗺️ **Roadmap** | What's coming next and what we're currently building |
| 🎉 **Show & Tell** | Share how you're using OdooDevTools, wins, workflows |
| 💬 **General** | Anything else — Odoo debugging tips, war stories, feedback |

---

## Before You Post a Bug

Please include:

1. **Odoo version** (e.g. 17.0, 16.0)
2. **Agent version** (run `odoodevtools-agent --version`)
3. **What you expected to happen**
4. **What actually happened**
5. **Any relevant logs** (agent logs or dashboard error messages)

---

## Roadmap Snapshot

Here's where the project stands today:

| Sprint | Focus | Status |
|---|---|---|
| Foundation + Auth + Multi-tenant | Core infrastructure | ✅ Done |
| Schema Engine | Schema snapshots + diffs | ✅ Done |
| Agent Pipeline + Error Tracking | Smart sampling, error grouping | ✅ Done |
| ACL Debugger | 5-stage access trace | ✅ Done |
| Profiler + Performance Budgets | Waterfall, N+1, compute chains | ✅ Done |
| Migration Scanner | v14→v18 breaking change detection | ✅ Done |
| Anonymizer + Retention | PII detection, data cleanup | 🔄 In Progress |

---

## Early Access

The product isn't publicly launched yet. If you're interested in early access or want to be notified at launch, drop a comment in the **General** discussion or reach out directly.

Feedback at this stage directly shapes what gets built next.

---

## A Note on the Repo

The source code is currently private. Discussions are open so the community can follow progress, report issues, and help shape the direction of the tool — even before public launch.

---

*Built with Go · PostgreSQL · Redis · WebSocket . Next JS With TypeScript*
