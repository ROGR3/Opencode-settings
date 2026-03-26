---
description: Run lints and tests, fix issues, report logic bugs
agent: verify
subtask: true
---

Run verification on this project.

Here are the recent changes for context:

!`git diff HEAD~1 --stat 2>/dev/null || git diff --stat 2>/dev/null || echo "No git history available"`

Start by reading the justfile to discover available lint and test commands, then run them.
