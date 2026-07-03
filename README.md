# AI & Agents in Accounting and Auditing

Portfolio of the AI agents [Vijay Vittal](https://linkedin.com/in/vijayvittals) builds for the accounting and auditing profession — plus the résumé behind them.

**Live site:** https://gitmaster-max.github.io/ai-agents-in-accounting/

## The agents

| # | Agent | Status | What it does | Links |
|---|---|---|---|---|
| 01 | **Audit Perspectives** | 🟢 Live | STORM-style (Shao et al., NAACL 2024) multi-stakeholder method for audit questions — perspective grid across the engagement team and external regulators, a tension map of where views conflict, and an actionable synthesis. | [Case study](https://gitmaster-max.github.io/ai-agents-in-accounting/agents/audit-perspectives.html) · [Live site](https://gitmaster-max.github.io/audit-perspectives/) · [Repo](https://github.com/gitmaster-max/audit-perspectives) |
| 02 | **Financial Statement Intelligence** | 🟡 Spec published | Upload a raw trial balance, get department-by-department readiness perspectives for FS preparation — AP/AR through the close process to the CFO — grounded in deterministic diagnostics and rolled up into a RAG scorecard. | [Agent instructions](https://gitmaster-max.github.io/ai-agents-in-accounting/agents/financial-statement-intelligence.html) |

## The method

Every agent in the collection follows four rules:

1. **Multi-perspective by design** — model the disagreement between stakeholders, not just the answer.
2. **Deterministic before generative** — where the input is data, findings come from computed diagnostics; the model interprets, it doesn't invent.
3. **Evidence behind every finding** — every conclusion cites an account, an amount, or a stated perspective.
4. **Shipped open, documented fully** — each agent publishes the actual instructions it runs on.

## Site structure

```
index.html                                  landing page: about, agents, method, contact
resume.html                                 full résumé (print/save-as-PDF ready)
agents/audit-perspectives.html              case study for agent 01
agents/financial-statement-intelligence.html  published spec for agent 02
styles.css                                  shared design system (light + dark)
site.js                                     theme toggle, scroll reveal
404.html                                    "this page doesn't reconcile"
```

No framework, no build step, no external dependencies. Deploys automatically via GitHub Pages from `main`.

## Adding a new agent

1. Create `agents/<agent-name>.html` (copy an existing agent page for the chrome).
2. In `index.html`, copy an `<article class="agent-card">` block into the `agent-grid`, before the `coming-soon` card. Set the agent number, status pill (`status-live` / `status-dev`), description, and links.
3. Add a row to the table above.
4. Commit and push — GitHub Pages redeploys automatically.

## Contact

**Vijay Vittal** — Assistant Audit Manager at EY · CPA (WA) · CMA
[vijayvittal98@gmail.com](mailto:vijayvittal98@gmail.com) · [LinkedIn](https://linkedin.com/in/vijayvittals) · [GitHub](https://github.com/gitmaster-max)
