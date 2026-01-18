# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a **Claude Code plugin** containing a skill that transforms Claude into a 3HAG strategic planning coach. It implements Shannon Susko's "3HAG WAY" framework — a 12-step strategic execution system for creating 3-year business plans.

## Structure

```
├── .claude-plugin/
│   ├── plugin.json             # Plugin metadata (name, version, author)
│   └── marketplace.json        # Marketplace catalog for distribution
├── skills/
│   └── 3hag-coach/
│       ├── SKILL.md            # Skill definition (frontmatter + coaching instructions)
│       └── references/
│           ├── methodology.md  # Complete 12-step 3HAG process
│           └── tools.md        # Templates for all strategic tools
```

## How It Works

- `plugin.json` defines the plugin metadata for installation via `/plugin install`
- `marketplace.json` allows users to add this repo as a plugin source
- `SKILL.md` frontmatter (`name:`, `description:`) defines when the skill activates
- The skill triggers on strategic planning keywords: 3HAG, Core Customer, swimlanes, Activity Fit Map, Market Map, One Phrase Strategy

## Key Concepts

**3HAG** = 3 Year Highly Achievable Goal — close enough to be tangible, far enough to be strategic

**The 12 Steps**: Foundation → Gut It Out → Key Function Flow → Market Map → Core Customer → Attribution Framework → Activity Fit Map L1 → One Phrase Strategy → Activity Fit Map L2 → Swimlanes → 36-Month Forecast → Confirm

**Widgets/Profit/X**: The single economic denominator (e.g., profit per customer, profit per employee)

**Session types**: Full 3HAG creation, single tool focus, or review (monthly/quarterly/annual)

## Output Artifacts

When coaching, the skill creates markdown documents in the user's repo at `docs/strategy/`:
- `3hag.md` — Master document
- `core-customer.md`, `market-map.md`, `attribution-framework.md`, `activity-fit-map.md`, `swimlanes.md`, `forecast.md`

Templates for all artifacts are in `skills/3hag-coach/references/tools.md`.

## Coaching Approach

Use Socratic questioning rather than providing answers. Complete each step before moving to the next. Push back on vague or conflicting answers. Every session should produce a tangible artifact.
