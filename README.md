# RLY Marketing — Claude plugin

A Claude Code plugin for the Properly team. It **writes and evaluates Properly marketing copy** for website, blog, LinkedIn, and X — in the brand voice, on-trend, and without sounding AI-generated. Every draft ships with a scorecard.

## What's inside

The `rly-marketing-copy` skill bundles:

- **Voice & Format Guide** — the frozen brand voice, the Five Rules, banned words, per-channel format/length, and the only approved list of client numbers and proof points.
- **Storytelling toolkit** — hooks, PAS/BAB/StoryBrand, show-don't-tell, rhythm.
- **Anti-AI-tells layer** — banned words, structural/tonal/rhythm tells, and a pre-ship checklist so nothing reads machine-written.
- **Topic packs** — 10 trend/theme packs (ETF, RWA, stablecoins, regulated crypto, open finance, agentic finance, fraud, and more) with keywords, dated angles, ready-made theses, and the clients that anchor each theme.
- **Scorecard** — scores every draft 1–5 on trend fit, persona fit, and master-prompt compliance, with a verdict and ranked fixes.

## Install (Claude Code / Claude Desktop)

```
/plugin marketplace add Properly-DEV/rly-marketing
/plugin install rly-marketing-copy@rly-marketing
/reload-plugins
```

Verify with `/plugin list`. The skill then triggers automatically when you ask for Properly copy, or on demand via `/rly-marketing-copy`.

### Stay up to date automatically

Add this to your `.claude/settings.json` so you always get the latest version on the next session:

```json
{
  "extraKnownMarketplaces": {
    "rly-marketing": {
      "source": { "source": "github", "repo": "Properly-DEV/rly-marketing" },
      "autoUpdate": true
    }
  }
}
```

## How to brief it

Name the channel and the subject in one line: *"LinkedIn post about the Axi rebrand"* or *"draft the branding page H1/H2."* The skill will confirm the **core message** before writing, so the post says something specific instead of something generic. To review an existing draft instead of writing, say *"score this post"* or *"is this on-brand"* — it returns the scorecard.

## Two rules everyone must know

1. **Numbers about Properly's work come only from the guide's §5.** If a figure isn't there, it's invented — cut it or swap in a real one.
2. **Market stats in the topic packs are external context, not Properly results.** They're dated third-party figures; verify before publishing and never present one as our outcome.

## Updating the plugin (maintainers)

Edit files under `plugins/rly-marketing-copy/skills/rly-marketing-copy/`, bump `version` in both `.claude-plugin/marketplace.json` and `plugins/rly-marketing-copy/.claude-plugin/plugin.json`, commit, and push. Teams with `autoUpdate` on get it on their next session.

## Structure

```
.claude-plugin/marketplace.json          # marketplace catalog
plugins/rly-marketing-copy/
├── .claude-plugin/plugin.json           # plugin manifest
└── skills/rly-marketing-copy/           # the skill
    ├── SKILL.md
    ├── references/  (voice guide, storytelling, anti-ai-tells, scorecard)
    ├── examples/
    └── topics/      (10 trend packs + index)
```
