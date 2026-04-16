# Keyword Research Dashboard — Sidekick Digital Skill

A Claude Skill that teaches Claude how to run end-to-end keyword research for a client, output a branded HTML dashboard, and deploy it live to Railway via GitHub.

## What this skill does

When a Sidekick team member says something like:

- "Do keyword research for [client]"
- "Build a keyword dashboard for [niche]"
- "Update the keyword research for [existing client]"

Claude will:

1. Gather a brief (client name, niche, audience, must-include themes)
2. Pull volume + CPC data from DataForSEO (Google Ads source)
3. Cross-reference with Semrush for zero-volume keywords
4. Group keywords into 4–8 intent-based ad groups
5. Flag zero-volume client-requested terms as exact-match placeholders (don't silently drop them)
6. Output a single-file HTML dashboard using the BRĒTH v2 template styling
7. Commit to a GitHub repo → Railway auto-deploys → share the live URL

## How to install

**Option A: Upload to Claude.ai (Team/Enterprise plan)**
1. Download this `skills/keyword-research/` folder as a .zip
2. Claude.ai → Settings → Capabilities → Skills → Upload Skill
3. Share org-wide

**Option B: Use with Claude Code or API**
Point Claude at this directory via the Agent SDK's skills loader.

## Files

- `SKILL.md` — the brain. Process, instructions, output format
- `template_dashboard.html` — the BRĒTH v2 HTML template Claude matches
- `example_brief.md` — what a good client brief looks like
- `deploy_instructions.md` — GitHub + Railway deploy steps

## Maintained by

Sidekick Digital. Last updated April 16, 2026.
