# 3HAG Coach Plugin for Claude Code

A Claude Code skill that coaches users through Shannon Susko's **3HAG (3 Year Highly Achievable Goal)** strategic planning framework from "3HAG WAY: The Strategic Execution System."

## What it does

This skill turns Claude into an experienced 3HAG coach that guides you through strategic planning using Socratic questioning. It helps you:

- **Create a full 3HAG** — Walk through all 12 steps of the framework
- **Work on individual tools** — Focus on specific exercises like Core Customer, Market Map, or Swimlanes
- **Review existing plans** — Monthly, quarterly, and annual reviews of your strategy

## 3HAG Framework Overview

The 3HAG methodology creates a "3 Year Highly Achievable Goal" — close enough to be tangible, far enough to be strategic. It includes:

1. Foundation (Core Purpose, Values, BHAG, Profit/X)
2. Gut It Out — Initial 3-year targets
3. Key Function Flow Map
4. Market Map (Porter's Five Forces)
5. Core Customer Profile
6. Attribution Framework — Competitive white space analysis
7. Activity Fit Map — Your differentiators
8. One Phrase Strategy
9. Swimlanes — 12-quarter roadmap
10. 36-Month Rolling Forecast
11. Brand Promise with Guarantee
12. Confirm Your 3HAG

## Installation

### Via Plugin Marketplace (recommended)

```bash
# Add the marketplace
/plugin marketplace add rsanaie/3hag-coach-plugin

# Install the plugin
/plugin install 3hag-coach
```

### Manual Installation

```bash
# Clone and symlink
git clone https://github.com/rsanaie/3hag-coach-plugin.git
ln -s "$(pwd)/3hag-coach-plugin/skills/3hag-coach" ~/.claude/skills/3hag-coach
```

## Usage

The skill activates automatically when you discuss strategic planning topics. You can also invoke it directly:

```
Help me create a 3HAG for my company
```

```
I want to define my Core Customer
```

```
Let's build a Market Map for my competitive landscape
```

```
Review my existing 3HAG plan
```

## Artifacts

The skill creates markdown documents in your repository at `docs/strategy/`:

| File | Purpose |
|------|---------|
| `3hag.md` | Master 3HAG document |
| `core-customer.md` | Core Customer Profile |
| `market-map.md` | Porter's Five Forces analysis |
| `attribution-framework.md` | Competitive attribute analysis |
| `activity-fit-map.md` | Differentiators and supporting activities |
| `swimlanes.md` | 12-quarter milestone roadmap |
| `forecast.md` | 36-month rolling forecast |

## Credits

Based on Shannon Susko's book "3HAG WAY: The Strategic Execution System that ensures your strategy is not a Wild-Ass-Guess!"

## License

MIT License — see [LICENSE](LICENSE)
