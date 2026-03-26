---
description: Generate a commit message from the currently staged files
---
Current branch:
!`git branch --show-current`
Here are the currently staged changes:
!`git diff --cached`
Based on the staged diff above, generate a concise and meaningful git commit message following these rules:
1. Use conventional commit format: `type(scope): description`
   - Types: feat, fix, refactor, docs, test, chore, style, perf, ci, build
   - Scope is optional but encouraged
2. The first line (subject) must be under 72 characters
3. Focus on the **why**, not the **what** -- the diff already shows what changed
4. If there are multiple logical changes, suggest separate commits
5. Add a body (separated by blank line) only if the change is complex
Output ONLY the commit message(s), no extra commentary.