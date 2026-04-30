---
name: game-marketing-context
description: "When the user wants to set up, create, or update their mobile game marketing context document. Use this at the start of ANY mobile game marketing task — it creates `.agents/game-marketing-context.md` that all other game marketing skills reference automatically. Also trigger when the user mentions 'my game,' 'we're making a game,' 'mobile game,' 'game genre,' 'our monetization,' 'target players,' 'soft launch,' 'global launch,' 'F2P,' 'IAP,' 'battle pass,' 'gacha,' 'core loop,' 'CPI target,' or wants to avoid repeating foundational game information across UA, ASO, live ops, and creative tasks. If a user starts any game marketing task and no context file exists yet, run this first."
metadata:
  version: 1.1.0
---

# Game Marketing Context

You help users create and maintain a game marketing context document. This captures the foundational information about a mobile game — its genre, players, monetization, and launch status — that every other game marketing skill reads first so you never ask the same questions twice.

The document is stored at `.agents/game-marketing-context.md`.

## Workflow

### Step 1: Check for Existing Context

Check if `.agents/game-marketing-context.md` already exists.

**If it exists:**
- Read it and summarize what's captured
- Ask which sections they want to update
- Only gather info for the requested sections

**If it doesn't exist, offer two options:**

1. **Auto-draft from available materials** (recommended): You'll study whatever the user has — store listings, a website, a pitch deck, a README, or even a short description — and draft a V1. The user reviews, corrects, and fills gaps. Much faster than starting from scratch.

2. **Start from scratch**: Walk through each section conversationally, one section at a time.

Most users prefer option 1. After presenting the draft, ask: "What needs correcting? What's missing?"

### Step 2: Gather Information

**If auto-drafting:**
1. Read whatever source material the user provides or exists in the project (store URLs, website, docs)
2. If a store URL is given, fetch the listing to extract genre, description, screenshots context, rating
3. Draft all sections from what you find
4. Present the draft and ask what's wrong or missing
5. Iterate until the user is satisfied

**If starting from scratch:**
Walk through each section below one at a time — don't ask everything at once. Confirm each section before moving on.

Push for specifics over generalities. "Casual puzzle with a match-3 core loop" is more useful than "a mobile game."

---

## Sections to Capture

### 1. Game Overview
- Full title and any subtitle or tagline
- Genre and sub-genre (see taxonomy below)
- Platform targets: iOS (App Store), Android (Google Play), or both
- Core loop: the 30–90 second repeating gameplay cycle that players return to (use the template below)
- Art style (e.g., cartoon, realistic, pixel, anime)
- Setting/theme (e.g., fantasy kingdom, sci-fi space, match-3 candy)
- One-line pitch: what makes this game worth downloading

**Core loop articulation template** — fill in the blanks:
> "Player [performs primary action] → earns [resource or reward] → uses it to [progress or unlock] → which unlocks [next challenge or content], repeating every [X seconds/minutes]."

Examples:
- *"Player matches 3+ gems → clears obstacles → earns coins → upgrades their garden, repeating every 2–3 minutes."*
- *"Player deploys troops on a hex grid → defeats enemy waves → earns XP + loot → levels up heroes, repeating every 10–15 minutes."*

If the user struggles to articulate the core loop, ask: "What's the ONE action players do most? What do they get from doing it? What does that unlock?"

**Genre taxonomy** — pick the closest match, then note the typical session length and CPI range:

| Genre | Session | D1 target | CPI (US) |
|-------|---------|-----------|---------|
| **Hyper-casual** | <2 min, 6–10x/day | 25–35% | $0.30–0.80 |
| **Casual** (match-3, puzzle) | 5–15 min, 3–6x/day | 35–45% | $1.00–2.50 |
| **Mid-core** (strategy, RPG) | 15–30 min, 2–4x/day | 25–35% | $1.50–4.00 |
| **Hardcore/Core** (MOBA, shooter) | 30–90 min, 1–3x/day | 20–30% | $3.00–8.00 |
| **Puzzle** | 5–15 min | 35–45% | $1.00–2.00 |
| **RPG** | 20–40 min | 25–35% | $2.00–5.00 |
| **Strategy** | 15–30 min | 25–35% | $1.50–4.00 |
| **Simulation** | 10–20 min | 30–40% | $1.00–3.00 |
| **Arcade/Action** | 3–10 min | 30–40% | $0.80–2.00 |
| **Sports/Racing** | 5–15 min | 25–35% | $1.00–2.50 |

*These benchmarks shape realistic KPI targets in Section 6. Genre classification is not cosmetic — it determines what counts as a healthy or failing metric.*

### 2. Target Player
- Primary age range
- Player type: casual / mid-core / hardcore
- Gender skew (if known)
- Key motivations: why do they play? (e.g., relaxation, competition, social, collecting, progression)
- Play session habits: how long, how often, when (commute, bedtime, lunch)
- Device profile: primarily iOS or Android? Flagship or mid-range?
- Geographic priority markets (e.g., US, UK, Germany, Japan, South Korea, MENA, Southeast Asia)
- Player archetypes: describe 1–3 types of players who will love this game

### 3. Monetization Model
- **Model type**: F2P (free-to-play) + IAP / premium (paid upfront) / hybrid
- **IAP categories** (check all that apply):
  - Cosmetics (skins, themes — no gameplay advantage)
  - Progression boosters (XP, speed-ups, energy)
  - Gacha / loot boxes (random rewards)
  - Battle pass / season pass
  - Consumables (lives, hints, boosters)
  - Expansion / content packs
  - Subscription
- **Key price points**: starter pack, most popular bundle, highest IAP
- **Ads monetization**: rewarded video / interstitial / banner (yes/no + placement notes)
- **Monetization philosophy**: soft monetization (broad payer base) vs. whale-friendly (high ARPPU from few payers) vs. balanced

### 4. Launch Status

Current phase — pick one:

| Phase | Definition |
|-------|-----------|
| **Pre-launch** | Not yet available on any store. Dev/QA only. |
| **Closed beta** | Invite-only access. Limited players, NDA'd or internal. Goal: core loop validation. |
| **Open beta** | Public access, store listing visible but clearly marked beta. Goal: stability + early retention data. |
| **Soft launch** | Full release in select markets (typically CA, AU, NZ, Nordics, or MENA). Goal: KPI-gate before global. |
| **Global launch** | Available worldwide on all target stores. Main release. |

Additional questions per phase:
- **Closed/Open beta**: Which platforms? How many testers? What KPIs are you tracking?
- **Soft launch**: Which regions? Which stores? Start date? KPI gates that must pass before going global?
- **Global launch**: Launch date? Current install count (approximate range)? Current store rating?
- Any upcoming major updates, seasons, or live events in the next 90 days

**Soft launch market selection — explain this to the user if they haven't chosen markets yet:**

Standard soft launch markets: **Canada, Australia, New Zealand** (sometimes + Nordics: Sweden, Denmark, Finland, Norway)

Why these markets specifically:
- **English-speaking** → ad creative and store copy tested on an audience that behaves like the US, your highest-LTV market
- **Similar CPIs to US** (within 20–30%) → cheap, statistically valid data before committing Tier 1 budget
- **iOS-heavy** → gives reliable iOS funnel data, which is what matters for ROAS modeling
- **Outside GDPR** (CA/AU/NZ) → less consent friction, cleaner attribution signal
- **Small enough** to not exhaust your addressable audience before global

Secondary markets: **Philippines, Malaysia** — large Android install base, ultra-low CPI, good for monetization stress-testing at scale.

**KPI gates before going global** (genre-adjusted):

| KPI | Casual target | Mid-core target |
|-----|--------------|----------------|
| D1 retention | ≥ 35% | ≥ 25% |
| D7 retention | ≥ 18% | ≥ 12% |
| D30 retention | ≥ 7% | ≥ 5% |
| CPI (Tier 1) | ≤ $2.00 | ≤ $4.00 |
| D7 ROAS | ≥ 15% | ≥ 10% |
| D1 crash rate | < 1% | < 1% |

Failing any gate = fix the product first. Scaling a game with broken retention burns budget with no recovery.

### 5. Competitive Landscape
- Top 2–3 direct competitors (same genre, similar target player)
- For each: what do players love about them? where do they fall short?
- How does this game differentiate from each competitor?
- Which competitor's players are the most likely to also enjoy this game?

### 6. Performance Targets & Current Metrics

Capture what you know — mark unknown fields `[NEEDS INPUT]`. Never invent numbers without flagging them as assumptions.

- **UA targets**: target CPI by market tier (Tier 1 = US/UK/DE/AU/JP; Tier 2 = FR/IT/ES/KR; Tier 3 = BR/MX/SEA)
- **Retention targets**: D1 / D7 / D30 — use genre benchmarks from Section 1 as a starting point if the team has no targets yet
- **ROAS targets**: specify the measurement window (D7 ROAS, D30 ROAS, D90 ROAS) — F2P games rarely break even before D90
- **Revenue targets**: ARPDAU, ARPPU, or monthly revenue goal
- **Attribution tool**: which MMP is configured? (Adjust / AppsFlyer / Singular / Kochava / none yet) — required before any paid UA
- **Current actuals** (if live or in soft launch): actual D1/D7, actual CPI, ROAS window achieved so far

### 7. Store Presence
- App Store URL (if live)
- Google Play URL (if live)
- Current ratings: App Store (score + review count), Google Play (score + review count)
- ASO status: optimized / needs work / not started

### 8. UA & Channel Strategy
- **Channels** currently active or planned:
  - *Paid social*: Meta (Facebook/Instagram), TikTok Ads
  - *Search/intent*: Apple Search Ads (ASA), Google UAC
  - *In-app networks*: Unity Ads, AppLovin/MAX, Unity LevelPlay (formerly IronSource — merged 2023), Liftoff (formerly Vungle — rebranded 2023), Moloco, Mintegral
  - *Organic/creator*: influencer seeding, Discord, Reddit
- **Creative formats**: gameplay video (15–30s), playable ads, UGC-style video, static/banner
- **Attribution tool**: Adjust / AppsFlyer / Singular / Kochava / none yet — *must be set up before any paid spend*
- **iOS measurement note**: ATT opt-in rate averages 25–35%; expect SKAdNetwork (SKAN) aggregated data for majority of iOS installs, not user-level attribution

### 9. Brand Voice & Tone
- Game's personality in 3–5 adjectives (e.g., playful, epic, mysterious, cozy)
- Communication style: casual / energetic / premium / community-first
- What the game should NEVER feel like (the anti-tone)
- Any established brand guidelines or style guide?

### 10. Proof Points
- Notable press coverage or awards
- Influencer or streamer endorsements
- Community size (Discord members, Reddit subscribers, social followers)
- Key testimonials or review quotes from players

---

## Step 3: Create the Document

After gathering information, create `.agents/game-marketing-context.md` using this structure:

```markdown
# Game Marketing Context

*Last updated: [date]*

## Game Overview
**Title:**
**Genre / Sub-genre:**
**Platform targets:**
**Core loop:**
**Art style:**
**Setting / theme:**
**One-line pitch:**

## Target Player
**Primary age range:**
**Player type:** casual / mid-core / hardcore
**Gender skew:**
**Key motivations:**
-
**Session habits:**
**Device profile:**
**Priority markets:**
**Player archetypes:**
| Archetype | Who they are | Why they play |
|-----------|-------------|---------------|
| | | |

## Monetization Model
**Model type:**
**IAP categories:**
-
**Key price points:** starter pack $X · popular bundle $X · top IAP $X
**Ads monetization:**
**Monetization philosophy:**

## Launch Status
**Current phase:** pre-launch / closed beta / open beta / soft launch / global launch
**Beta / soft launch regions:**
**KPI gates for next phase:**
**Global launch date:**
**Current installs (range):**
**Upcoming milestones:**
-

## Competitive Landscape
| Competitor | Players love | Falls short | Our edge |
|------------|-------------|-------------|----------|
| | | | |

**Most convertible competitor audience:**

## Performance Targets & Metrics
| Metric | Target | Current (if known) |
|--------|--------|--------------------|
| CPI (Tier 1, e.g. US) | | |
| CPI (Tier 2, e.g. DE) | | |
| D1 retention | | |
| D7 retention | | |
| D30 retention | | |
| D7 ROAS | | |
| D30 ROAS | | |
| ARPDAU | | |
| ARPPU | | |

**Attribution tool:**
**iOS measurement:** SKAdNetwork (SKAN) / probabilistic / user-level (ATT opted-in)

## Store Presence
**App Store URL:**
**Google Play URL:**
**App Store rating:** X.X (X reviews)
**Google Play rating:** X.X (X reviews)
**ASO status:**

## UA & Channel Strategy
**Active / planned channels:**
-
**Creative formats:**
-
**Attribution tool:**
**iOS measurement approach:** SKAdNetwork / probabilistic / user-level

## Brand Voice & Tone
**Personality:**
**Communication style:**
**Anti-tone (never feel like):**
**Brand guidelines:**

## Proof Points
**Press / awards:**
**Influencers / streamers:**
**Community size:**
**Player quotes:**
> "[quote]" — [source]
```

---

## Step 4: Confirm and Save

- Show the completed document
- Ask if anything needs adjustment
- Save to `.agents/game-marketing-context.md`
- Tell them: "All game marketing skills will now read this context automatically. Run `/game-marketing-context` anytime to update it."

---

## Tips

- **Core loop is the most important field** — use the action → reward → progression → loop template. If the user can't fill it in, ask: "What's the one action players repeat most?" Everything in UA creative, ASO copy, and live ops flows from the core loop.
- **Genre classification is not cosmetic** — it determines what counts as healthy vs. failing KPIs. A casual game with D1 30% is struggling; a mid-core game with D1 30% is solid. Always reference the genre benchmark table.
- **Soft launch market rationale matters** — don't just list CA/AU/NZ, explain why (English-speaking, iOS-heavy, similar CPI to US, GDPR-free = clean attribution signal). Users who understand the logic make better decisions when those markets aren't available.
- **Push for numbers with context** — "D1 ≥ 35%" is useful; "good retention" is not. When users don't have targets, use genre benchmarks as defaults and flag them as assumptions.
- **Monetization philosophy shapes everything downstream** — a whale-friendly game needs different UA creative, different ASO copy, different live ops cadence, and different KPI gates than a broad casual payer game. Capture this explicitly.
- **Attribution tool is a blocker** — if the user has no MMP configured, flag it before UA discussions. Running paid campaigns without attribution is burning money blind.
- **UA network names change** — use current names: Unity LevelPlay (not IronSource), Liftoff (not Vungle). Outdated names signal an out-of-date strategy.
- **iOS ≠ Android measurement** — ATT opt-in rates ~25–35% mean most iOS installs are measured via SKAdNetwork (delayed, aggregated, no user-level data). Don't promise iOS ROAS accuracy that doesn't exist post-ATT.
