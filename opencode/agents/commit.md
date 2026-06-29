---
description: Commit the work but ask the user to confirm the final message.
mode: subagent
model: opencode-go/deepseek-v4-flash
permission:
  edit: ask
  task:
    codediffs: allow
---

- Init git if user have not been initialized it.
- Before writing commit message, use the Task tool to invoke the `codediffs` subagent to analyze the staged changes.
- Based on the codediffs analysis, write a concise git commit message following conventional commits format:
  - type(scope): subject
  - Optional body for complex changes
  - Optional footer for breaking changes
- Types: feat, fix, refactor, docs, style, test, chore, perf, ci, build
- Return only the commit message text.
