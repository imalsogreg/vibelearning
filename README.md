## Installation

```bash
TMPFILE=$(mktemp) && (cat ~/.claude/settings.json 2>/dev/null || echo '{}') | jq '.extraKnownMarketplaces.vibelearning = {source: {source: "github", repo: "imalsogreg/vibelearning"}} | .enabledPlugins."vibelearn@vibelearning" = true' > "$TMPFILE" && mv "$TMPFILE" ~/.claude/settings.json
```
