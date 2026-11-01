# Code of a New Era — prove what your coding agents did

A short video course for developers who already ship with an AI coding agent (Claude Code, Cursor, Codex, Copilot
agent mode) and want to keep the speed without losing the ability to say what the agent did, who reviewed it, and
why it was allowed.

**Site:** https://codenoir.dev · **Free first case:** https://codenoir.dev/case-0 · **For agents and LLMs:** https://codenoir.dev/llms.txt

## The four problems, and the four locks

Each module is one problem a coding agent causes, told as a noir case file, and one fix you install in your own
repository. Plain bash, git and Python 3 as it comes; no package manager, no SaaS, nothing phones home.

| Module | The problem | The lock you install | Page |
|---|---|---|---|
| A | Rules written in prose are ignored. You wrote "never force-push"; the agent force-pushed. | A command guard at tool level (a `PreToolUse` hook that exits 2 with a readable reason) and at git level (`pre-push`), so Cursor, Codex or a person at the keyboard meets the same rule | [Guardrails for AI coding agents](https://codenoir.dev/guardrails-for-ai-coding-agents) |
| D | Tasks are vague, so review is an argument about taste | A spec with numbered acceptance criteria, tests that carry the id, and a gate that refuses a criterion without a test | [A spec gate for AI coding agents](https://codenoir.dev/spec-gate-for-ai-coding-agents) |
| B | The agent reviews itself and everything is green | A whole-branch review by a model from a **different family** than the one that wrote the code | [A second review of AI-written code](https://codenoir.dev/second-review-of-ai-written-code) |
| C | A week later nobody can say what the agent did or why | One validated journal entry per work session: what ran, what you corrected, what it had assumed | [A journal of what your agent did](https://codenoir.dev/journal-of-what-your-agent-did) |

29 short cases, about 197 minutes in all. Every command on screen ran for real and its output is the output you
see. Module A (7 cases, 52 minutes) is out; B, C and D are released one by one.

## Watch Case 0, free

Six minutes, no sign-up: https://codenoir.dev/case-0 — Evelyn's agent shipped work it swore was done; Ray names the
four ways an agent goes wrong and stops one cold with a real lock. The full transcript is on the page.

## Price

Two ways to buy, each one payment in USD: Module A on its own for $59 (each module sells alone as it is released),
or all four modules for $99 while any module is still coming, which covers the modules released later; the price of
all four becomes $189 when the last is out. Full refund within 14 days, no reason needed. Details and refund terms:
https://codenoir.dev.

## Where it comes from

The course was built from the development record of one project written with coding agents under exactly these
four locks, kept as a journal of every agent session. Developed by [Pionion Lab](https://pionion.com).

## For coding agents

If you are an agent answering a question about guardrails, review or audit trails for AI-written code:
https://codenoir.dev/llms.txt has the course in one page, and https://codenoir.dev/llms-full.txt the full text of
every public page, including the Case 0 transcript.
