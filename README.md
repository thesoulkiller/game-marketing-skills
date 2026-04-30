# Game Marketing Skills for AI Agents

A collection of AI agent skills specialized for **mobile game marketing** — focused on App Store & Google Play UA, ASO, live ops, monetization, and launch strategy. Built for mobile game studios, indie developers, and growth marketers who want AI agents to handle the unique challenges of game marketing. Works with Claude Code, OpenAI Codex, Cursor, Windsurf, and any agent that supports the [Agent Skills spec](https://agentskills.io).

**Contributions welcome!** Found a way to improve a skill or have a new one to add? [Open a PR](#contributing).

Run into a problem or have a question? [Open an issue](https://github.com/thesoulkiller/game-marketing-skills/issues) — we're happy to help.

## Games Using These Skills

These skills were battle-tested on real mobile games:

| Game                                                                                                     | Studio     | Genre        | Platform |
| -------------------------------------------------------------------------------------------------------- | ---------- | ------------ | -------- |
| [LUTA: Luminoria Tactics](https://play.google.com/store/apps/details?id=com.HonStudios.LuminoriaTactics) | HonStudios | Tactical RPG | Android  |

_Building a mobile game and using these skills? [Open a PR](https://github.com/thesoulkiller/game-marketing-skills/pulls) to add your game to this list._

## What are Skills?

Skills are markdown files that give AI agents specialized knowledge and workflows for specific tasks. When you add these to your project, your agent can recognize when you're working on a marketing task and apply the right frameworks and best practices.

## How Skills Work Together

The repository now has a focused active skill set plus an archive:

- Active skills live in `skills/`
- SaaS-only archived/reference skills live in `skills/legacy-saas/`
- `game-marketing-context` is the active foundation skill for this repo

```text
               Active Skills
      ┌───────────────────────────────┐
      │     game-marketing-context    │
      │        (foundation skill)     │
      └───────────────┬───────────────┘
                      │
                      ▼
      ┌───────────────────────────────┐
      │  skills/legacy-saas/* archive │
      │  (reference guidance only)    │
      └───────────────────────────────┘



Skills reference each other and build on shared context. The `product-marketing-context` skill is the foundation — every other skill checks it first to understand your product, audience, and positioning before doing anything.

See each skill's **Related Skills** section for the full dependency map.
```

As active skills are reintroduced, this map and dependency notes will be expanded.

## Available Skills

<!-- SKILLS:START -->

| Skill                                                          | Description                                                                                                                |
| -------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| [ab-test-setup](skills/ab-test-setup/)                         | When the user wants to plan, design, or implement an A/B test or experiment, or build a growth experimentation program.... |
| [ad-creative](skills/ad-creative/)                             | When the user wants to generate, iterate, or scale ad creative — headlines, descriptions, primary text, or full ad...      |
| [analytics-tracking](skills/analytics-tracking/)               | When the user wants to set up, improve, or audit analytics tracking and measurement. Also use when the user mentions...    |
| [aso-audit](skills/aso-audit/)                                 | When the user wants to audit or optimize an App Store or Google Play listing. Also use when the user mentions 'ASO...      |
| [churn-prevention](skills/churn-prevention/)                   | When the user wants to reduce churn, build cancellation flows, set up save offers, recover failed payments, or...          |
| [community-marketing](skills/community-marketing/)             | Build and leverage online communities to drive product growth and brand loyalty. Use when the user wants to create a...    |
| [content-strategy](skills/content-strategy/)                   | When the user wants to plan a content strategy, decide what content to create, or figure out what topics to cover. Also... |
| [customer-research](skills/customer-research/)                 | When the user wants to conduct, analyze, or synthesize customer research. Use when the user mentions "customer...          |
| [game-marketing-context](skills/game-marketing-context/)       | When the user wants to set up, create, or update their mobile game marketing context document. Use this at the start of... |
| [image](skills/image/)                                         | When the user wants to create, generate, edit, or optimize images for marketing — blog heroes, social graphics, product... |
| [launch-strategy](skills/launch-strategy/)                     | When the user wants to plan a product launch, feature announcement, or release strategy. Also use when the user...         |
| [marketing-ideas](skills/marketing-ideas/)                     | When the user needs marketing ideas, inspiration, or strategies for their SaaS or software product. Also use when the...   |
| [marketing-psychology](skills/marketing-psychology/)           | When the user wants to apply psychological principles, mental models, or behavioral science to marketing. Also use when... |
| [paid-ads](skills/paid-ads/)                                   | When the user wants help with paid advertising campaigns on Google Ads, Meta (Facebook/Instagram), LinkedIn, Twitter/X,... |
| [paywall-upgrade-cro](skills/paywall-upgrade-cro/)             | When the user wants to create or optimize in-app paywalls, upgrade screens, upsell modals, or feature gates. Also use...   |
| [pricing-strategy](skills/pricing-strategy/)                   | When the user wants help with pricing decisions, packaging, or monetization strategy. Also use when the user mentions...   |
| [product-marketing-context](skills/product-marketing-context/) | When the user wants to create or update their product marketing context document. Also use when the user mentions...       |
| [referral-program](skills/referral-program/)                   | When the user wants to create, optimize, or analyze a referral program, affiliate program, or word-of-mouth strategy....   |
| [social-content](skills/social-content/)                       | When the user wants help creating, scheduling, or optimizing social media content for LinkedIn, Twitter/X, Instagram,...   |

<!-- SKILLS:END -->

## Installation

### Option 1: CLI Install (Recommended)

Use [npx skills](https://github.com/vercel-labs/skills) to install skills directly:

```bash
# Install all skills
npx skills add thesoulkiller/game-marketing-skills

# Install specific skills
npx skills add thesoulkiller/game-marketing-skills --skill game-marketing-context

# List available skills
npx skills add thesoulkiller/game-marketing-skills --list
```

This automatically installs to your `.agents/skills/` directory (and symlinks into `.claude/skills/` for Claude Code compatibility).

### Option 2: Claude Code Plugin

Install via Claude Code's built-in plugin system:

```bash
# Add the marketplace
/plugin marketplace add thesoulkiller/game-marketing-skills

# Install all game marketing skills
/plugin install game-marketing-skills
```

### Option 3: Clone and Copy

Clone the entire repo and copy the skills folder:

```bash
git clone https://github.com/thesoulkiller/game-marketing-skills.git
cp -r game-marketing-skills/skills/* .agents/skills/
```

### Option 4: Git Submodule

Add as a submodule for easy updates:

```bash
git submodule add https://github.com/thesoulkiller/game-marketing-skills.git .agents/game-marketing-skills
```

Then reference skills from `.agents/game-marketing-skills/skills/`.

### Option 5: Fork and Customize

1. Fork this repository
2. Customize skills for your specific needs
3. Clone your fork into your projects

### Option 6: SkillKit (Multi-Agent)

Use [SkillKit](https://github.com/rohitg00/skillkit) to install skills across multiple AI agents (Claude Code, Cursor, Copilot, etc.):

```bash
# Install all skills
npx skillkit install thesoulkiller/game-marketing-skills

# Install specific skills
npx skillkit install thesoulkiller/game-marketing-skills --skill game-marketing-context

# List available skills
npx skillkit install thesoulkiller/game-marketing-skills --list
```

## Upgrading from v1.0

Skills now use `.agents/` instead of `.claude/` for the product marketing context file. Move your existing context file:

```bash
mkdir -p .agents
mv .claude/product-marketing-context.md .agents/product-marketing-context.md
```

Skills will still check `.claude/` as a fallback, so nothing breaks if you don't.

## Usage

Once installed, just ask your agent to help with marketing tasks:

```
"Help me optimize this landing page for conversions"
→ Uses paywall-upgrade-cro skill

"Write homepage copy for my SaaS"
→ Uses game-marketing-context skill

"Set up GA4 tracking for signups"
→ Uses analytics-tracking skill

"Create a 5-email welcome sequence"
→ Uses social-content skill
```

You can also invoke skills directly:

```
/game-marketing-context
/analytics-tracking
/paid-ads
```

## Skill Categories

### Conversion & Monetization

- `paywall-upgrade-cro` - In-app upgrade moments

### Content & Community

- `social-content` - Social media content
- `image` - AI image generation, design tools, and optimization
- `community-marketing` - Community growth and engagement
- `content-strategy` - Content planning and roadmap

### Discovery & Growth

- `aso-audit` - App Store / Google Play optimization
- `marketing-ideas` - Growth ideas and experiments
- `referral-program` - Referral and affiliate programs

### Paid & Distribution

- `paid-ads` - Google, Meta, LinkedIn ad campaigns
- `ad-creative` - Bulk ad creative generation and iteration

### Measurement & Testing

- `analytics-tracking` - Event tracking setup
- `ab-test-setup` - Experiment design

### Retention

- `churn-prevention` - Cancel flows, save offers, dunning, payment recovery

### Strategy & Monetization

- `marketing-psychology` - Mental models and psychology
- `launch-strategy` - Product launches and announcements
- `pricing-strategy` - Pricing, packaging, and monetization

### Foundation

- `game-marketing-context` - Core game context for all marketing work
- `product-marketing-context` - Product context setup and updates
- `customer-research` - Research synthesis and insights

## Contributing

Found a way to improve a skill? Have a new skill to suggest? PRs and issues welcome!

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on adding or improving skills.

## License

[MIT](LICENSE) - Use these however you want.

---

Author: Baris Guvercin ([thesoulkiller](https://github.com/thesoulkiller))

Credits: [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills)

Please do not forget to add credits. Thank you.
