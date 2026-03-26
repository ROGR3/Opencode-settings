---
description: Find unused functions, exports, and files, then ask before deleting
agent: dead-code
subtask: true
---

Scan this codebase for dead code -- unused functions, exports, variables, types, and files.

Project structure overview:

!`find . -type f \( -name "*.ts" -o -name "*.py" -o -name "*.go" -o -name "*.rs" -o -name "*.js" \) -not -path "*/node_modules/*" -not -path "*/.git/*" -not -path "*/dist/*" -not -path "*/__pycache__/*" | head -60`

Report all findings grouped by confidence level, then ask me what to remove.
