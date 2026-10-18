<p align="center">
  <img src="https://avatars.githubusercontent.com/u/270479298?v=4" width="120" height="120" alt="Aenea Labs" style="border-radius: 16px;">
</p>

<h1 align="center">Aenea Labs</h1>

<p align="center">
  <strong>Trustworthy building blocks for AI agents, and the systems built from them.</strong><br>
  <sub>Deterministic &middot; Auditable &middot; Human-approved &middot; Zero dependencies where the problem allows</sub>
</p>

---

Aenea Labs is the portfolio of **LaVon Rutledge**: AI agent infrastructure and security engineering, designed for regulated industries where every automated decision has to be explained, tested, and approved by a person.

## Project Aura

**[aenealabs/aura](https://github.com/aenealabs/aura)** &mdash; an autonomous AI security platform for enterprise codebases. Aura finds a vulnerability, writes the patch, proves it in a network-isolated sandbox, and queues it for human approval.

- Coder, Reviewer, and Validator agents with checks and balances, grounded in hybrid GraphRAG code context
- Human-in-the-loop approval workflows with industry-specific policy presets
- 26,000+ tests &middot; Python 3.11+ &middot; source available under BSL 1.1 (becomes Apache 2.0 on 2030-03-23)

## Agent packages

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

## Upcoming projects

- **Backlog Pilot** &mdash; an AI backlog copilot for product owners. It turns stakeholder requests into epics and stories that are traced to the stakeholder's own words, quality-checked, and WSJF-prioritized, with a person approving every AI suggestion. *In active development.*
- **Listening-tour synthesizer** *(working title)* &mdash; turns stakeholder interview notes into themes, personas, and a prioritized list of problems.
- **Status &amp; risk narrator** *(working title)* &mdash; drafts weekly leadership updates and early risk warnings from delivery, budget, and risk-log data.

## Principles

- **Regulated first.** Audit trails, human approval, and least privilege are designed in from the start; simpler environments get them for free.
- **Rules where trust matters.** Checks that must be trusted run as readable rules, not model judgment; model output is verified, not assumed.
- **Deterministic tests.** Recorded runs instead of live model calls, so tests are repeatable and cost nothing.
- **Nothing hidden.** Zero third-party dependencies in the libraries, CI on every package, and design decisions recorded as ADRs in Aura.

## About the name

Aenea Labs takes its name from Aenea, a central character in Dan Simmons's [*The Rise of Endymion*](https://en.wikipedia.org/wiki/The_Rise_of_Endymion) (1997), the fourth and final novel of the Hyperion Cantos. In the book, Aenea is the child of a human and an artificial intelligence.

---

<p align="center">
  <sub>Built and maintained by LaVon Rutledge &middot; <a href="https://github.com/aenealabs">github.com/aenealabs</a></sub>
</p>
