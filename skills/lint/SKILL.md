---
name: wiki-lint
description: Run this skill when the user asks to check the content quality of the wiki.
---

Use this skill as an instruction set. Follow the workflow in order.

## Workflow

Periodically, ask the LLM to health-check the wiki. Look for: contradictions between pages, stale claims that newer sources have superseded, orphan pages with no inbound links, important concepts mentioned but lacking their own page, missing cross-references, data gaps that could be filled with a web search. The LLM is good at suggesting new questions to investigate and new sources to look for. This keeps the wiki healthy as it grows.
