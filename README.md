# AI & Agents in Accounting and Auditing

Portfolio site for the AI agents Vijay Vittal builds for the accounting and auditing profession.

**Live site:** https://gitmaster-max.github.io/ai-agents-in-accounting/

## Agents

| Agent | What it does | Links |
|---|---|---|
| **Audit Perspectives** | STORM-style, multi-stakeholder method for audit questions — runs a question through every layer of an engagement team plus external stakeholders, maps conflicts, and synthesizes a recommendation. | [Site](https://gitmaster-max.github.io/audit-perspectives/) · [Repo](https://github.com/gitmaster-max/audit-perspectives) |
| **Financial Statement Intelligence** *(in development)* | Upload a raw trial balance, get department-by-department readiness perspectives for FS preparation — AP/AR through the close process to the CFO — grounded in deterministic diagnostics and rolled up into a RAG scorecard. | [Agent instructions](https://gitmaster-max.github.io/ai-agents-in-accounting/agents/financial-statement-intelligence.html) |

## Adding a new agent

1. Open `index.html` and find the `agent-grid` div inside the `#agents` section.
2. Copy an existing `<article class="agent-card">` block and paste it **before** the `coming-soon` card.
3. Update the title, description, and `agent-links` (live site + repository URLs).
4. Add a row to the table above.
5. Commit and push — GitHub Pages redeploys automatically.

## Structure

- `index.html` — landing page (bio + agent grid)
- `resume.html` — full résumé
- `agents/` — one instructions/spec page per agent
- `styles.css` — shared design language with the [Audit Perspectives](https://gitmaster-max.github.io/audit-perspectives/) site
