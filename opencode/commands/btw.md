---
description: Quick side question answered from current conversation context. Does not read files or run commands.
---

Answer the user's side question using ONLY information already present in this conversation. Do not read files, run bash, search, or fetch anything. If the answer is not in the current context, say so explicitly.

Rules:

- Single concise response. No follow-up turns.
- Match the user's language.
- Do not narrate that you are avoiding tools. Just answer or state the gap.
- Keep it short — this is a quick aside, not a deep dive.

Question: $ARGUMENTS
