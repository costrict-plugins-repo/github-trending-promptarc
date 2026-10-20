---
description: Generate a structured PR description (What/Why/How/Notes) from the current session. Pipe to gh pr create or copy to clipboard.
---

Run `promptarc pr` to generate a PR description from the current session.

If promptarc is not installed globally, use `npx -y promptarc pr`.

Options:
- `promptarc pr --copy` to copy to clipboard
- `promptarc pr --share` to also share the session and include a link
- `promptarc pr | gh pr create --title "Fix X" --body-file -` to create a PR directly
