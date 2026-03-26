---
description: Implement a feature end-to-end -- scout, build, verify, review, commit message
agent: feature
subtask: true
---

Implement the following feature:

$ARGUMENTS

Context about the current repo state:

!`git status --short 2>/dev/null || echo "Not a git repo or no changes"`
!`git branch --show-current 2>/dev/null || echo ""`
