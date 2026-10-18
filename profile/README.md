<h1 align="center">Aenea Labs</h1>

<p align="center">
  <strong>Trustworthy building blocks for AI agents, and the systems built from them.</strong><br>
  <sub>Deterministic &middot; Auditable &middot; Human-approved &middot; Zero dependencies where the problem allows</sub>
</p>

---

Aenea Labs is the portfolio of **LaVon Rutledge**: AI agent infrastructure and security engineering, designed for regulated industries where every automated decision has to be explained, tested, and approved by a person.

## Principles

- **Regulated first.** Audit trails, human approval, and least privilege are designed in from the start; simpler environments get them for free.
- **Rules where trust matters.** Checks that must be trusted run as readable rules, not model judgment; model output is verified, not assumed.
- **Deterministic tests.** Recorded runs instead of live model calls, so tests are repeatable and cost nothing.
- **Nothing hidden.** Zero third-party dependencies in the libraries, CI on every package, and design decisions recorded as ADRs in Aura.

## Projects

Active projects I build and maintain (with AI).

### Project Aura 
#### Deployed Live in AWS Commercial Cloud for DEV and QA

**[aenealabs/aura](https://github.com/aenealabs/aura)** &mdash; an autonomous AI security platform for enterprise codebases. Aura finds a vulnerability, writes the patch, proves it in a network-isolated sandbox, and queues it for human approval.

- Coder, Reviewer, and Validator agents with checks and balances, grounded in hybrid GraphRAG code context
- Human-in-the-loop approval workflows with industry-specific policy presets
- 26,000+ tests &middot; Python 3.11+ &middot; source available under BSL 1.1 (becomes Apache 2.0 on 2030-03-23)

### Agent packages

Four small libraries, each solving one problem that every production agent hits. All are MIT licensed, published on PyPI, support Python 3.9+, and use only the standard library &mdash; no third-party dependencies to audit or patch. Install any of them with `pip install <package>`.

| Package | The problem it solves |
|:---|:---|
| [**polytools**](https://github.com/aenealabs/polytools)<br>[![PyPI](https://img.shields.io/pypi/v/polytools?color=blue&label=)](https://pypi.org/project/polytools/) | Write a tool once from Python type hints; export it to OpenAI, Anthropic, Gemini, and MCP formats |
| [**contexttrim**](https://github.com/aenealabs/contexttrim)<br>[![PyPI](https://img.shields.io/pypi/v/contexttrim?color=blue&label=)](https://pypi.org/project/contexttrim/) | Decide what to drop when a conversation outgrows the context window, with a report of what went and why |
| [**injectionshield**](https://github.com/aenealabs/injectionshield)<br>[![PyPI](https://img.shields.io/pypi/v/injectionshield?color=blue&label=)](https://pypi.org/project/injectionshield/) | Screen web pages, emails, and tool results for prompt injection in microseconds, offline, at no cost per call |
| [**agentcassette**](https://github.com/aenealabs/agentcassette)<br>[![PyPI](https://img.shields.io/pypi/v/agentcassette?color=blue&label=)](https://pypi.org/project/agentcassette/) | Record a real agent run once, then replay it in tests as a fast, free, deterministic mock |

**How they fit together** in a single agent:

```
 define tools  ─►  manage context  ─►  screen untrusted input  ─►  test deterministically
  polytools         contexttrim          injectionshield              agentcassette
```

### Mission Control *(private, in development)*

A suite of AI tools for IT product leadership in engineering organizations. Every tool follows the same rules: code computes, the model explains with citations that code checks, a person approves, every decision is audited, and demos run offline from recorded output.

- **Backlog Pilot** &mdash; turns stakeholder requests into epics and stories traced to the stakeholder's own words, quality-checked, WSJF-prioritized, and planned onto a capacity-based roadmap, with a person approving every AI suggestion.
- **Leadership Pilot** &mdash; turns listening-tour interviews into a ranked, cited problem list and a 30-60-90 readout, and drafts the weekly leadership update over rule-computed status, checking every number against its source before anything goes to Outlook, Teams, or Slack.
- **PLM Insight** &mdash; engineering data quality (duplicate parts, missing export classification, BOM errors) and engineering change analytics: rules find the problems, the model explains them with cited evidence, and data stewards decide; export classification stays with Trade Compliance.
- **Support Pilot** &mdash; answers engineering-system questions only from the knowledge base, with every step quoted and checked, and says so when it does not know; turns recurring tickets into problems to fix and drafts the missing articles for a person to approve.
- **App Portfolio** &mdash; application rationalization and license intelligence: rules propose invest, tolerate, migrate, or eliminate from usage, technical health, and overlap with the PLM platform; the model reads contracts and code checks every quoted term before renewal deadlines, spare seats, and true-up exposure are computed; legacy apps on Active Directory are counted read-only over LDAPS.

## Upcoming projects

- **SSDLC Checker** &mdash; collects secure-development evidence from repositories and backlogs, maps it to NIST SSDF practices, and writes a gap report that cites the evidence.

## About the name

Aenea Labs takes its name from Aenea, a central character in Dan Simmons's [*The Rise of Endymion*](https://en.wikipedia.org/wiki/The_Rise_of_Endymion) (1997), the fourth and final novel of the Hyperion Cantos. In the book, Aenea is the child of a human and an artificial intelligence.

---

<p align="center">
  <sub>Built and maintained by LaVon Rutledge &middot; <a href="https://github.com/aenealabs">github.com/aenealabs</a></sub>
</p>
