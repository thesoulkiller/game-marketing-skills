# Mobile Game Marketing Knowledge Base

*Synthesized from Adjust guides, industry benchmarks, and mobile gaming best practices.*
*Sources: Adjust.com guides (mobile game marketing, video ads, privacy laws, game development, PC/console), AppsFlyer State of Gaming, Data.ai (App Annie), SensorTower, GameAnalytics benchmarks, Segwise.ai (AI in Mobile Game Marketing & Advertisement — 2024/2025 data), Liftoff Mobile Gaming Apps Report.*

---

## How to Use This Document

All game marketing skills in this repo should be evaluated against this knowledge base. When building or reviewing a skill:

1. **Check terminology** — does the skill use correct mobile game industry vocabulary? (see Glossary)
2. **Check benchmarks** — does the skill reference realistic KPI targets? (see Benchmarks by Genre)
3. **Check privacy compliance** — does the skill account for ATT, SKAdNetwork, and consent requirements?
4. **Check ad formats** — does the skill recommend the right creative formats for games?
5. **Check launch phases** — does the skill correctly distinguish soft launch from global launch KPI gates?

---

## 1. Mobile Game UA Fundamentals

### The UA Funnel for Games
```
Impression → Click → Install → Tutorial Complete → Day 1 Return → First Purchase → Long-term Retention
```

Each step has a benchmark drop-off. Skills must not conflate web marketing funnels (leads, MQLs, SQLs) with this install-based funnel.

### Core UA Metrics — Required Vocabulary

| Metric | Definition | Why It Matters |
|--------|-----------|----------------|
| **CPI** | Cost Per Install — total spend ÷ installs | Primary efficiency metric for UA campaigns |
| **CPM** | Cost Per Mille — cost per 1,000 ad impressions | Bidding baseline for programmatic |
| **CTR** | Click-Through Rate — clicks ÷ impressions | Creative engagement signal |
| **IR** | Install Rate — installs ÷ clicks | Store listing + ad alignment signal |
| **ROAS** | Return on Ad Spend — revenue ÷ spend | Profitability metric; typical window: D7, D14, D30 |
| **LTV / LCV** | Lifetime Value — total revenue from a player cohort | Foundation of UA bid decisions |
| **ARPU** | Average Revenue Per User | LTV precursor; measure at D7, D30, D180 |
| **ARPPU** | Average Revenue Per Paying User | Monetization depth signal |
| **ARPDAU** | Average Revenue Per Daily Active User | Daily monetization health |
| **DAU / MAU** | Daily/Monthly Active Users | Engagement health |
| **DAU/MAU ratio** | Stickiness — how often monthlies return daily | >20% = healthy; >40% = excellent |
| **D1 / D7 / D30** | Day 1/7/30 retention rates | Most critical KPIs before global launch |
| **IPM** | Installs Per Mille — installs per 1,000 impressions | Creative performance benchmark for video ads |
| **eCPM** | Effective CPM — revenue per 1,000 impressions (publisher side) | Monetization metric for ad-supported games |
| **CAC** | Customer Acquisition Cost | Same as CPI in gaming context |
| **LTV:CAC ratio** | LTV divided by CAC | >3x = profitable UA; <1x = losing money |

### UA Network Landscape (Current, 2025)

| Network | Best For | Notes |
|---------|---------|-------|
| **Meta (Facebook/Instagram)** | Broad targeting, lookalikes, video | Highest volume; impacted by ATT but strong ML |
| **Google UAC** | Android-first, YouTube, Play Store | Auto-optimizes across Search/Play/YouTube/Display |
| **Apple Search Ads (ASA)** | iOS intent-based discovery | Highest-intent iOS users; IDFA-exempt |
| **TikTok Ads** | Hyper-casual, younger demographics, UGC creatives | Fast-growing; strong for casual/hyper-casual |
| **Unity Ads** | Mid-core, rewarded video in-game | Strong rewarded inventory; Unity LevelPlay mediation |
| **AppLovin/MAX** | Mid-core to hardcore; mediation + UA | MAX mediation + AppLovin Exchange; strong ROAS optimization |
| **IronSource → Unity LevelPlay** | Merged with Unity 2023; SDK-based mediation | No longer a standalone network |
| **Liftoff (formerly Vungle)** | Casual to mid-core, creative automation | Vungle rebranded to Liftoff Monetize 2023 |
| **Moloco** | ML-based programmatic; strong for scaling | Excellent for mid-core once LTV data exists |
| **Mintegral** | Asia-Pacific markets; strong China/SEA reach | Useful for APAC expansion |
| **Chartboost** | Legacy mid-core network; now owned by Zynga/Take-Two | Declining relevance |
| **Digital Turbine** | Carrier/OEM pre-install campaigns | Unique distribution; device-level targeting |

**Attribution tools:** Adjust, AppsFlyer, Singular, Kochava. Every serious UA program needs one. Never run campaigns without attribution.

---

## 2. Benchmarks by Genre

These are industry medians. Skills must reference these ranges rather than making up numbers.

### Retention Benchmarks (D1 / D7 / D30)

| Genre | D1 | D7 | D30 |
|-------|----|----|-----|
| Hyper-casual | 25–35% | 8–12% | 2–4% |
| Casual (match-3, puzzle) | 35–45% | 15–25% | 6–12% |
| Mid-core (strategy, RPG) | 25–35% | 12–20% | 5–10% |
| Hardcore / Core (MOBA, shooter) | 20–30% | 10–18% | 5–10% |
| Casino / Social casino | 30–40% | 15–20% | 5–8% |

*Source: GameAnalytics Mobile Gaming Benchmarks, AppsFlyer State of Gaming*

### CPI Benchmarks by Market (2024–2025)

| Market | Hyper-casual | Casual | Mid-core | Hardcore |
|--------|-------------|--------|---------|---------|
| USA (Tier 1) | $0.30–0.80 | $1.00–2.50 | $1.50–4.00 | $3.00–8.00 |
| UK / Germany / AU | $0.25–0.70 | $0.80–2.00 | $1.20–3.50 | $2.50–7.00 |
| Japan / South Korea | $0.40–1.00 | $1.20–3.00 | $2.00–6.00 | $4.00–10.00 |
| Brazil / Mexico | $0.10–0.30 | $0.30–0.80 | $0.50–1.50 | $1.00–3.00 |
| SEA (ID/TH/VN) | $0.05–0.20 | $0.15–0.50 | $0.30–1.00 | $0.80–2.00 |

*Higher CPI markets = higher LTV. Scale in Tier 1 only once LTV:CAC ≥ 3x is proven in soft launch.*

### ROAS Targets (Return on Ad Spend)

| Window | Target |
|--------|--------|
| D7 ROAS | 20–30% of spend recovered |
| D30 ROAS | 50–70% of spend recovered |
| D90 ROAS | 80–110% (breakeven range) |
| D180+ ROAS | >130% (profitable) |

*F2P games rarely recover spend before D30. UA profitability is a long game.*

### Session Benchmarks

| Genre | Avg Session Length | Sessions/Day |
|-------|------------------|-------------|
| Hyper-casual | 1–3 min | 6–10 |
| Casual | 5–15 min | 3–6 |
| Mid-core | 15–30 min | 2–4 |
| Hardcore | 30–90 min | 1–3 |

---

## 3. Mobile Video Ads in Games

### Ad Format Hierarchy (by effectiveness for games)

| Format | Completion Rate | eCPM Range | Best For |
|--------|----------------|-----------|---------|
| **Rewarded Video** | 85–95% | $8–25 CPM | All genres; highest engagement |
| **Playable Ads** | N/A (interactive) | $10–30 CPM | Mid-core, strategy games |
| **Interstitial Video** | 60–75% | $4–15 CPM | Hyper-casual, casual |
| **Offerwall** | Completion-based | Variable | RPG, strategy (high-LTV) |
| **Native/Banner** | Low | $0.50–3 CPM | Fill / supplemental only |

### Rewarded Video Best Practices
- **Placement**: between sessions (level end > level start), never mid-gameplay
- **Opt-in**: always user-initiated; never forced for F2P games
- **Reward**: must be meaningful — 5 coins is worse than no ad
- **Frequency cap**: 3–5 rewarded videos per session max
- **Paywall escape**: rewarded video as alternative to IAP is the highest-converting placement

### Video Ad Creative Benchmarks (UA-side)
- **Optimal length**: 15–30 seconds for interstitial; playables 30–60s
- **First 3 seconds**: must hook immediately — 60%+ of drop-off happens here
- **Gameplay footage**: authentic gameplay outperforms polished cinematic for mid-core
- **UGC-style**: low-fi "real player" footage performs best on TikTok / Meta for casual
- **End card**: always include clear CTA ("Download Free" > "Play Now" > generic CTA)
- **Sound-off assumption**: 85% of mobile video watched on mute — captions essential
- **Aspect ratios**: 9:16 for TikTok/Stories; 1:1 for feed; 16:9 for YouTube

### Playable Ads
- Show the ACTUAL core loop, not a dumbed-down demo
- Keep interaction count to 3–5 taps maximum
- Target ROAS is 30–50% higher than standard video for mid-core
- Best networks: ironSource (Unity LevelPlay), AppLovin, Mintegral

### IPM Benchmarks
| Format | Weak | Average | Strong |
|--------|------|---------|--------|
| Video (15s) | <2 | 3–6 | >8 |
| Video (30s) | <1.5 | 2–4 | >6 |
| Playable | <3 | 5–10 | >15 |

*IPM = installs per 1,000 impressions. Kill creatives below threshold; scale above.*

---

## 4. Launch Phases and KPI Gates

### Phase Definitions

| Phase | Definition | Goal |
|-------|-----------|------|
| **Pre-production** | Concept, prototyping | Validate core loop fun |
| **Closed Beta** | Invite-only, internal/NDA testers | Core loop stability, crash rates |
| **Open Beta** | Public but flagged as beta | Early retention signal, bug discovery |
| **Soft Launch** | Full release in select markets | KPI-gate before global spend |
| **Global Launch** | Worldwide release | Scale UA profitably |

### Soft Launch Market Selection Logic
Standard soft launch markets: **Canada, Australia, New Zealand, Nordics (Sweden/Denmark/Finland/Norway)**

Why these markets:
- English-speaking = valid creative test for US campaigns
- iOS-heavy = iOS funnel data (highest LTV market)
- Similar CPIs to US (within 20–30%) but lower competition = cheaper data
- GDPR does not apply (CA/AU/NZ) — less consent friction vs. EU markets
- Large enough for statistical significance; small enough to not "use up" virgin audiences

Secondary soft launch markets: **Philippines, Malaysia** (large Android user base, low CPI, good stress-test for monetization at scale before global)

### KPI Gates Before Global Launch

These are the thresholds a game must hit in soft launch before scaling UA globally:

| KPI | Casual | Mid-core | Note |
|-----|--------|---------|------|
| D1 retention | ≥ 35% | ≥ 25% | Core loop test |
| D7 retention | ≥ 18% | ≥ 12% | Habit formation test |
| D30 retention | ≥ 7% | ≥ 5% | Long-term product test |
| CPI (Tier 1) | ≤ $2.00 | ≤ $4.00 | Acquisition efficiency |
| D7 ROAS | ≥ 15% | ≥ 10% | Early monetization signal |
| Day-1 crash rate | < 1% | < 1% | Technical stability |

*Failing any gate = fix the product before scaling. Scaling a broken game burns budget with no recovery.*

---

## 5. Privacy Laws and Their Impact on Mobile UA

### Key Regulations

| Law | Region | Key Impact on UA |
|-----|--------|-----------------|
| **GDPR** | EU/EEA | Consent required before tracking; right to deletion; data minimization |
| **CCPA/CPRA** | California, USA | Opt-out of sale of personal data; "Do Not Sell" requirement |
| **ATT** (App Tracking Transparency) | iOS globally | Opt-in consent required for cross-app tracking on iOS 14.5+ |
| **COPPA** | USA | No behavioral tracking for under-13; age gates required |
| **PEGI/ESRB ratings** | EU/USA | Content rating affects app store categorization and ad targeting restrictions |

### Apple's ATT (App Tracking Transparency) — Critical for iOS UA

- **What it did**: Requires explicit opt-in before using IDFA (Apple's device identifier) for cross-app tracking
- **Opt-in rates**: Industry average 25–35% consent. ~65–75% of iOS users are unmeasurable via IDFA
- **Impact**: Severely reduced iOS attribution accuracy. Meta's ROAS reporting inflated; actual ROAS lower
- **Solutions**:
  - **SKAdNetwork (SKAN)**: Apple's privacy-preserving attribution framework; 24–48h delayed, aggregated, no user-level data
  - **SKAN 4.0**: Improved (2023) — hierarchical conversion values, web-to-app support
  - **Probabilistic modeling**: MMPs (Adjust, AppsFlyer) use modeled attribution to fill IDFA gaps
  - **Apple Search Ads**: IDFA-exempt — ASA data is the most reliable iOS signal
  - **First-party data**: Push notification opt-in, account registration → more reliable signals

### SKAdNetwork Limitations to Know
- Conversion window: 24h (SKAN 3) / configurable (SKAN 4)
- No user-level data — only campaign-level aggregated conversion counts
- Conversion values: 6-bit (0–63 values) in SKAN 3; fine/coarse values in SKAN 4
- Postback delay: 24–48h minimum; nulls when install volume too low
- Skills must not assume real-time iOS attribution — it doesn't exist post-ATT

### Android Attribution
- Google's Privacy Sandbox replacing GAID (Google Advertising ID) gradually
- Android attribution still more reliable than iOS (2024–2025 transition period)
- Google's Attribution API: aggregated, privacy-preserving — similar trajectory to SKAN
- GAID opt-out rate: ~15–20% (much lower than iOS ATT)

### Consent Management Best Practices for Games
- Use a **CMP (Consent Management Platform)**: OneTrust, Usercentrics, Didomi
- GDPR consent gate must appear before SDK initialization in EU
- For under-13 games (COPPA): disable all behavioral ads; use contextual ads only
- Age gate at session start for PEGI 16/18 or ESRB M/AO rated games
- In-game privacy policy link required by both app stores

---

## 6. ASO (App Store Optimization) for Games

### iOS App Store — Game-Specific Rules

- **Category**: Games → sub-category (Action, Adventure, Casual, Puzzle, Racing, Role Playing, Simulation, Sports, Strategy, Trivia, Word)
- **In-app events**: Games use these for seasonal events, new content drops, tournaments — they appear in search results and featured sections
- **Subtitle**: Include genre keyword + core differentiator (e.g., "Strategy RPG · Build & Battle")
- **Screenshots**: First screenshot = most critical. Show the most exciting gameplay moment, not a title screen
- **App preview video**: Games see the highest conversion lift from video — 20–40% more installs. Show core gameplay within first 3 seconds.
- **Keyword field (100 bytes)**: Never repeat words from title/subtitle. Target secondary keywords and genre modifiers.

### Google Play — Game-Specific Rules

- **Category**: Game → sub-category (matches iOS categories roughly)
- **Short description (80 chars)**: Indexed and visible in search — treat like a meta description
- **Full description**: IS indexed. Use natural language with keyword density 2–3%. Structure: hook → core loop → features → social proof.
- **Feature graphic**: Required for any featured placement. Games with compelling feature graphics get 2–4x more installs when featured.
- **Tags**: Google Play allows adding gameplay tags (e.g., "Strategy", "Tower Defense", "Offline") — use all available
- **Ratings**: Games below 4.0 see significant install conversion drop-off. 4.2+ is the target floor.

### Huawei App Gallery (HMS)
- Separate keyword indexing system from Google/Apple
- AppGallery Connect console for ASO management
- Key in MENA, Eastern Europe, and China-adjacent markets
- HMS Core must be integrated (alternative to Google Mobile Services)
- Games need separate HMS Analytics and HMS Ads SDK integration
- Featured placement program ("Editors' Choice") is accessible to quality games

---

## 7. Monetization Models

### F2P Monetization Architecture

| Model | Description | Best Genre Fit |
|-------|-------------|---------------|
| **Consumables** | Coins, gems, lives, energy — spent and repurchased | Casual, hyper-casual |
| **Gacha / Loot boxes** | Random reward pulls; collection mechanics | Mid-core RPG, strategy |
| **Battle Pass** | Seasonal premium track; paid + free tiers | Mid-core, hardcore |
| **Cosmetics only** | Skins, themes — zero pay-to-win | Competitive / hardcore |
| **Progression boosters** | Speed-ups, XP boosts, skip timers | Strategy, simulation |
| **Expansion packs** | New chapters, worlds, content | Puzzle, casual RPG |
| **Subscription** | Monthly/annual premium membership | Casual (Candy Crush, Bejeweled) |
| **Ads + IAP hybrid** | Rewarded video + optional IAP | Hyper-casual to casual |

### Payer Segmentation (Whale Curve)
- ~1–3% of players make 50–80% of revenue — these are **whales**
- ~5–10% make one small purchase — **minnows / occasional payers**
- ~90%+ never pay — monetized via ads or not at all

**Implication for skills**: Pricing strategy for games is about maximizing whale spend AND converting minnows, not about broad subscription adoption like SaaS.

### Starter Pack Psychology
- First purchase offer shown within first 24–72 hours of play
- Best price point: $0.99–$4.99 (removes psychological barrier to paying)
- Content: 5–10x value vs. normal price (perceived value, not real cost)
- Time-limited: "Offer expires in 23:47:XX" — deadline drives conversion
- Conversion rate: 2–8% of engaged D1 players who see the offer

### IAP Price Localization
Currency-adjust prices per market — do not just convert USD. Use Apple's/Google's pricing tiers.
| Market | Typical top IAP | Starter pack |
|--------|----------------|-------------|
| USA | $99.99 | $0.99–4.99 |
| Japan | ¥9,800 (~$65) | ¥120–480 |
| Germany | €79.99 | €0.99–3.99 |
| Brazil | R$39.90 (~$8) | R$4.90 |
| SEA | $4.99–9.99 | $0.99 |

---

## 8. PC/Console vs. Mobile Marketing — Key Differences

Skills in this repo are **mobile-only**. If a user mentions PC or console, flag the differences:

| Dimension | Mobile | PC/Console |
|-----------|--------|-----------|
| Distribution | App stores (gated) | Steam, Epic, PSN, Xbox (more open) |
| UA channels | Meta, Google UAC, TikTok, DSPs | YouTube, Twitch, Discord, influencers, PR |
| Attribution | MMP required (Adjust, AppsFlyer) | Steam analytics, first-party |
| Monetization | F2P IAP dominant | Premium + DLC dominant; F2P growing |
| Discovery | ASO (keyword-driven) | Steam tags, Metacritic, content creators |
| Launch | Soft launch → global (phased) | Simultaneous global usually |
| Install friction | 1-tap install | Download/install, PC spec requirements |
| Session length | Short (mobile) | Long (PC/console) |
| UA cost | CPI $0.20–$10 | CAC $5–$50+ |

---

## 9. Skill Evaluation Checklist

Use this checklist when evaluating any new or updated skill in this repo:

### Terminology Check
- [ ] Uses CPI not "cost per lead" or "CPL"
- [ ] Uses D1/D7/D30 retention not "churn rate" or "engagement"
- [ ] Uses LTV not "customer value" (or qualifies it properly)
- [ ] Uses correct UA network names (Unity LevelPlay not IronSource; Liftoff not Vungle)
- [ ] Distinguishes iOS and Android attribution differences (ATT impact on iOS)
- [ ] Uses F2P / IAP / monetization vocabulary correctly
- [ ] Refers to "players" not "customers" or "users" (except in analytics context)

### Benchmark Sanity Check
- [ ] CPI targets fall within genre-appropriate ranges (see Section 2)
- [ ] Retention targets fall within genre-appropriate ranges (see Section 2)
- [ ] ROAS targets use appropriate time windows (D7, D30, D90)
- [ ] Does not set unrealistic targets (D1 >60% is extraordinary; D30 >20% is extreme)

### Privacy Compliance Check
- [ ] Acknowledges ATT impact on iOS measurement
- [ ] Does not assume IDFA availability for iOS campaigns
- [ ] References SKAdNetwork for iOS attribution
- [ ] Mentions consent requirements for EU traffic (GDPR)
- [ ] Flags COPPA for games rated for children

### Launch Phase Check
- [ ] Correctly sequences: closed beta → open beta → soft launch → global launch
- [ ] Soft launch markets are justified (CA/AU/NZ logic explained)
- [ ] KPI gates before global are genre-specific (not one-size-fits-all)
- [ ] Does not recommend full-scale UA spend before KPI gates are passed

### Creative Check
- [ ] Recommends gameplay footage over cinematic for UA video
- [ ] Specifies rewarded video as primary in-app ad format
- [ ] Mentions playable ads for mid-core games
- [ ] Accounts for sound-off viewing (captions)
- [ ] References appropriate aspect ratios per platform

### Monetization Check
- [ ] Does not apply SaaS pricing logic to IAP design
- [ ] Understands whale/minnow segmentation
- [ ] Includes starter pack timing and psychology
- [ ] Addresses price localization by market

---

## 10. Glossary — Quick Reference

| Term | Definition |
|------|-----------|
| **ATT** | App Tracking Transparency — Apple's opt-in consent framework for IDFA |
| **IDFA** | Identifier for Advertisers — Apple's device ID (requires ATT consent) |
| **GAID** | Google Advertising ID — Android equivalent of IDFA |
| **SKAdNetwork / SKAN** | Apple's privacy-preserving attribution API |
| **MMP** | Mobile Measurement Partner — attribution tool (Adjust, AppsFlyer, Singular) |
| **Mediation** | SDK that runs waterfall/bidding auctions across ad networks (MAX, LevelPlay) |
| **Waterfall** | Legacy ad mediation pricing: networks queued by historical eCPM |
| **In-app bidding** | Real-time auction replacing waterfall; higher eCPMs for publishers |
| **Soft launch** | Controlled release in select markets to gather KPI data |
| **KPI gate** | Retention/monetization threshold that must be met before scaling |
| **Core loop** | The primary 30–90s repeating gameplay action players return to |
| **Meta loop** | Higher-level progression system above the core loop (base building, story, social) |
| **Rewarded video** | Opt-in video ad that grants in-game currency/items on completion |
| **Playable ad** | Interactive mini-demo of the game shown as an ad |
| **eCPM** | Effective cost per mille — revenue per 1,000 ad impressions (publisher metric) |
| **IPM** | Installs per mille — installs per 1,000 ad impressions (UA creative metric) |
| **ROAS** | Return on ad spend — revenue generated per dollar of UA spend |
| **LTV** | Lifetime value — total revenue expected from a player over their lifetime |
| **ARPPU** | Average revenue per paying user |
| **ARPDAU** | Average revenue per daily active user |
| **Whale** | Top spender segment; 1–3% of players, 50–80% of revenue |
| **Starter pack** | First-purchase offer shown to new players; deeply discounted |
| **Battle pass** | Seasonal paid track with escalating rewards for playtime |
| **Gacha** | Randomized reward system (loot boxes); regulated in some markets |
| **Live ops** | Live operations — real-time events, limited-time offers, seasonal content |
| **ASO** | App Store Optimization — equivalent of SEO for app stores |
| **Creative fatigue** | Performance decline when an ad is shown too many times to the same audience |
| **Lookalike audience** | Targeting users who statistically resemble your best existing players |
| **Re-engagement** | UA campaigns targeting lapsed players to return to the game |
| **Deep link** | URL that opens a specific in-game screen directly from an ad |
| **Deferred deep link** | Deep link that works even if the app isn't installed yet (install first, then route) |
| **CMP** | Consent Management Platform — handles GDPR/ATT consent flows |
| **AdAttributionKit** | Apple's next-generation attribution API, successor to SKAdNetwork (iOS 17.4+) |
| **Privacy Sandbox** | Google's replacement for GAID on Android — privacy-preserving attribution |
| **Incrementality** | Causal measurement — the lift in installs/revenue directly caused by an ad campaign |
| **MMM** | Marketing Mix Modeling — statistical method to attribute revenue across channels without user-level data |
| **pLTV** | Predicted Lifetime Value — ML-estimated LTV for a player cohort, often used for bid optimization |
| **Hybrid monetization** | Revenue model combining ad revenue and IAP (e.g., rewarded ads + starter packs) |
| **LGPD** | Brazil's Lei Geral de Proteção de Dados — similar scope to GDPR, affects Brazilian users |
| **DPDP Act** | India's Digital Personal Data Protection Act — consent and processing requirements for Indian users |
| **APRA** | American Privacy Rights Act — US federal privacy bill trajectory; impacts UA targeting if passed |
| **Cross-progression** | Shared player save data across platforms (e.g., mobile + PC) |
| **Crossplay** | Multiplayer between players on different platforms (mobile, PC, console) |
| **Cloud gaming** | Streaming games from remote servers to any device — removes install friction |
| **Session depth** | Number of game sessions per day per DAU; indicator of engagement beyond retention |
| **Hybrid video-playable** | Ad format that combines a video hook with an interactive playable outro |
| **LTO** | Limited-Time Offer — in-game IAP deal with a countdown timer to create urgency |
| **Event-driven re-engagement** | Push/ad campaigns tied to live ops events to bring lapsed players back |
| **KPI gate** | Retention/monetization threshold that must be met before scaling spend (see Section 4) |
| **Conversion value** | SKAN/AdAttributionKit signal mapping revenue or engagement events to a numeric post-install value |
| **DCO** | Dynamic Creative Optimization — AI automatically swaps creative elements (characters, text, scenes) per user segment in real time |
| **Creative velocity** | Rate at which new ad creative variants are produced, tested, and rotated; high velocity is required at UA scale |
| **Holdout test** | A/B test where the control group receives no ad — measures true causal lift (incrementality) vs. organic return |
| **UGC-style ads** | Ads designed to look like user-generated content; raw, authentic aesthetic correlates with high retention-linked install quality |
| **Lo-fi / ugly ads** | Low-production, deliberately rough ad creatives (screen recordings, hand-drawn assets) — high perceived authenticity, lower CPM |
| **Performance Max** | Google's ML-driven campaign type; auto-generates and distributes creatives across all Google surfaces |
| **Advantage+** | Meta's ML-driven campaign product; autonomously allocates budget across Facebook/Instagram placements |
| **Creative tagging** | Automated labeling of visual, text, and audio elements in ad assets to surface which creative components drive installs |
| **Churn prediction model** | Supervised ML model trained on historical player activity to score active players' likelihood of lapsing |
| **AI segmentation** | ML-based audience clustering by behavioral signals (session data, spend, progression) — beyond demographic targeting |
| **Deterministic MTA** | Multi-touch attribution using verified device matches (IDFA, email) — available for ~39% of iOS users |
| **Probabilistic attribution** | Assigns conversion probabilities using aggregated non-personal signals — required for the 61% of iOS without IDFA consent |
| **Creative fatigue window** | Typical performance decline point; at scale, expect meaningful CTR/IPM degradation after 3–5 days |
| **Deep linking (retargeting)** | Linking re-engagement ads directly to the exact game context (level, store, event) — ~3× conversion vs. generic homepage link |

---

## 11. New Skill Qualification Protocol (Mobile Game Marketing)

Use this protocol when reviewing any **new** skill before it is accepted into this repo.
The goal is to ensure each skill is not just "marketing-correct," but specifically fit for **mobile game growth**.

### 11.1 What to extract from a new skill draft

For each new skill, capture these elements first:

1. **Primary use case** (UA, ASO, monetization, creative, live ops, retention, re-engagement, launch planning, privacy)
2. **Target game subgenre** (hyper-casual, casual, mid-core, hardcore, social casino)
3. **Primary market focus** (Tier 1, Tier 2, APAC, global)
4. **KPI model used** (CPI, D1/D7/D30, ROAS windows, LTV/ARPDAU, etc.)
5. **Measurement assumptions** (MMP support, SKAN/AdAttributionKit handling, Android Privacy Sandbox awareness)
6. **Monetization assumptions** (ads, IAP, subscription, hybrid)

If the draft skill does not clearly define these six items, it is incomplete.

### 11.2 Pass/Fail Gate (must pass all)

#### Gate A — Mobile gaming specificity
- [ ] Uses game-native language (`players`, `sessions`, `core loop`, `live ops`, `D1/D7/D30`)
- [ ] Avoids SaaS/B2B-only framing (`MQL`, `SQL`, lead funnels) unless explicitly translated for games
- [ ] Differentiates genre behavior (e.g., hyper-casual vs. mid-core retention and monetization logic)

#### Gate B — KPI realism
- [ ] Benchmarks map to ranges in Section 2 (or clearly states "market/context dependent")
- [ ] Uses time-windowed ROAS (`D7`, `D30`, `D90`) rather than immediate profitability assumptions
- [ ] Includes a "stop/scale" decision rule (what to kill, what to iterate, what to scale)

#### Gate C — Privacy and attribution readiness
- [ ] Explicitly acknowledges ATT and partial iOS observability
- [ ] References SKAN/AdAttributionKit for iOS measurement constraints
- [ ] Includes consent/CMP logic where relevant (GDPR, CCPA/CPRA, APRA trajectory, COPPA)
- [ ] Avoids requiring user-level deterministic attribution as a hard dependency

#### Gate D — Creative and placement quality
- [ ] Follows format-specific guidance (rewarded/interstitial/playable/hybrid)
- [ ] Defines placement timing rules (natural breaks, no core-loop interruption)
- [ ] Mentions creative testing cadence (hook tests, variation, fatigue monitoring)
- [ ] Includes platform-fit constraints (sound-off, aspect ratio, channel-native style)

#### Gate E — Measurement and optimization design
- [ ] Defines core metrics for monitoring (at minimum: retention + revenue, not one in isolation)
- [ ] Includes segmentation/cohort logic (new vs. returning, payer segments, market splits)
- [ ] Recommends mediation/measurement stack where relevant
- [ ] Contains an experimentation loop (hypothesis -> test -> readout -> rollout)

If any checkbox in A-E fails, the skill should not be approved without revision.

### 11.3 Scoring rubric (0-100)

Use this weighted score to compare multiple candidate skills:

| Category | Weight | Scoring guidance |
|----------|--------|------------------|
| Mobile gaming specificity | 20 | 0 = generic marketing, 10 = partly game-aware, 20 = deeply game-native |
| KPI and benchmark accuracy | 20 | 0 = unrealistic, 10 = mixed, 20 = fully benchmark-aligned |
| Privacy and attribution readiness | 20 | 0 = ignores privacy reality, 10 = partial, 20 = robust and current |
| Execution quality (creative + channel + ops) | 20 | 0 = abstract advice only, 10 = some tactics, 20 = actionable and format-correct |
| Optimization design (testing + measurement loop) | 20 | 0 = no iteration logic, 10 = basic, 20 = clear operating system |

**Approval thresholds**
- **90-100**: Ready to ship
- **75-89**: Ship with minor edits
- **60-74**: Significant revision required
- **<60**: Reject and rewrite

### 11.4 Required "evidence block" in every new skill

Each new skill should include a short validation block with:
- **Assumed game type and market**
- **Primary KPI tree** (e.g., `CPI -> D1 -> D7 -> D30 -> D30 ROAS`)
- **Top 3 failure modes** (e.g., creative fatigue, ad over-frequency, weak early retention)
- **Iteration plan** (what to test next if KPI target fails)

This prevents "advice-only" skills and forces operational thinking.

### 11.5 Red flags requiring immediate rewrite

- Recommends scaling UA without soft launch KPI gates
- Treats all genres as having similar retention and monetization behavior
- Uses outdated platform naming as current (e.g., standalone IronSource/Vungle framing)
- Assumes full iOS user-level attribution post-ATT
- Optimizes ad revenue without any retention guardrail
- Treats PC/console channel logic as interchangeable with mobile without qualification

### 11.6 Suggested review workflow for maintainers

1. Run Section 9 checklist.
2. Run Section 11 pass/fail gates.
3. Compute Section 11 score (0-100).
4. Add revision notes tied to failed gates only.
5. Re-review after edits; approve only at 75+ with no failed mandatory gate.

This workflow keeps skill quality consistent as the knowledge base expands.

---

### 11.7 Contributor skill template (copy-paste into new SKILL.md)

Copy this block into the top of every new skill under the frontmatter. Fill in each field before writing instructions.

```markdown
<!--
SKILL QUALIFICATION BLOCK — required before review

Primary use case: [UA | ASO | monetization | creative | live ops | retention | re-engagement | launch | privacy]
Target subgenre:  [hyper-casual | casual | mid-core | hardcore | social casino | all]
Primary market:   [Tier 1 (US/UK/DE/AU/JP) | Tier 2 | APAC | global]

KPI tree:         [e.g. CPI → D1 retention → D7 retention → D30 ROAS]
Measurement:      [MMP required? SKAN/AdAttributionKit constraints? Android Privacy Sandbox aware?]
Monetization:     [ads | IAP | subscription | hybrid — specify mix]

Top 3 failure modes:
1. [e.g. creative fatigue on Meta after week 2]
2. [e.g. rewarded video placed mid-core-loop causing D1 drop]
3. [e.g. no ATT fallback → iOS data gap misread as campaign underperformance]

Iteration plan if KPI target fails:
- If D1 < target → [action]
- If CPI > target → [action]
- If D7 ROAS < target → [action]

Qualification score (self-assessed): [0-100] / Notes: [any caveats]
-->
```

**Rules:**
- The block is a markdown comment — it never renders for end users
- Do not submit a PR without filling every field
- Scores below 75 require a note explaining what is intentionally out of scope

---

### 11.8 Quick evaluation examples

Use these to calibrate the scoring rubric.

#### Example A — Strong skill (score ~88)

A `ua-strategy` skill that:
- Opens with genre selection and CPI/ROAS benchmarks per Section 2
- Includes separate UA network recommendations for iOS (ASA-first due to ATT) vs. Android
- Addresses SKAN conversion value setup and D7 modeling lag
- Specifies rewarded vs. interstitial placement windows with session-depth guidance
- Ends with a weekly optimization cadence: creative refresh at >3x weekly impressions, kill <IPM threshold

**What keeps it from 100**: no COPPA/GDPR step for age-gated games, no APAC market variant.

#### Example B — Weak skill (score ~42)

A `paid-ads` skill (unmodified from a SaaS base) that:
- References "lead generation" and "conversion funnels" without game translation
- Sets a flat "target CPI of $2" without genre or market qualification
- Recommends Facebook and Google but does not address ATT or SKAN
- Has no mention of creative formats, rewarded ads, or playables
- No iteration plan beyond "optimize your ads"

**Fails gates**: A (SaaS language), B (flat benchmark), C (no privacy awareness), D (no format guidance), E (no optimization loop).

#### Example C — Borderline skill (score ~67)

A `live-ops` skill that:
- Correctly identifies LTO (limited-time offers), battle pass cadence, and event-driven re-engagement
- Uses correct game vocabulary throughout
- But: no attribution or measurement guidance for live ops lift measurement
- No genre differentiation (hyper-casual live ops ≠ mid-core guild events)
- Treats all markets as having the same event timing (ignores APAC peak hours, Ramadan sensitivity, etc.)

**Verdict**: Revise to add measurement design and market/genre variants before approving.

---

## 12. AI-Powered Tools in Mobile Game Marketing (2024–2025)

*Source: Segwise.ai, Liftoff, AppsFlyer, Adjust 2025 projections.*

This section covers AI tooling that is now considered standard practice in mobile game UA. Skills that touch UA, creative, or retargeting should reflect this reality.

---

### 12.1 Market-level AI adoption benchmarks

| Signal | 2024 Data Point |
|--------|----------------|
| Mobile game in-app purchase revenue | ~$80 billion globally |
| YoY growth in mobile game advertisers | +60.4% to 259,700 |
| Growth in ad assets produced | +15.4% to 46.2 million |
| Impressions per DAU trend | Doubling year over year |
| iOS CPI trend (Q1'23–Q2'24) | Down ~17% (SKAN optimization improvement) |
| Android CPI trend (same period) | Up ~48% (demand surge, Privacy Sandbox friction) |
| iOS vs Android CPI ratio | iOS ~3.5× more expensive on average |
| iOS D7 ROAS (Liftoff data) | ~5.9% — slightly higher than Android |
| IDFA opt-in rate for games | 39% (highest category; still leaves 61% unresolvable) |
| AI UGC video cost | ~$7/video, 15 videos in <1 hour |
| CPI reduction from AI-generated UGC | ~40% in tested cases |
| Conversion rate lift from AI personalization | 10–15% |
| ROI lift from accurate segmentation | 20–35% higher (Segwise/industry data) |
| Retargeting with AI segmentation (Bagelcode case) | ARPU +33% from dormant high-LTV cohort |
| Deep-linked vs generic link conversion | ~3× higher conversion |

---

### 12.2 AI technologies now standard in mobile game UA

#### Predictive analytics and LTV modeling
- ML models ingest session length, play frequency, and purchase history to predict player LTV and churn risk
- AI-powered LTV bidding: bid aggressively on lookalike profiles of predicted high-LTV users, suppress low-value segments
- Tools: Liftoff LTV Optimize, AppsFlyer SKAN modeled conversions, Adjust's probabilistic attribution

#### ML-powered bidding platforms
| Platform | Mechanism |
|----------|-----------|
| **Google Performance Max** | Automates bids and dynamically generates ad assets across Search, Display, YouTube, Discover, Gmail, Maps |
| **Meta Advantage+** | Allocates spend across Facebook/Instagram placements; shifts budget based on live performance signals |
| **Moloco** | Independent ML DSP; no walled-garden data dependency; strong for non-Google/Meta scale |
| **AppLovin MAX** | Bidding mediation layer; ML-optimized waterfall replacement for publisher-side monetization |

#### Dynamic Creative Optimization (DCO)
- AI automatically swaps characters, scenes, or text overlays based on user history and segment
- DCO tools show players "what they missed" (last level, character, in-game store item) to maximize re-engagement click-through
- Seasonal/themed creative variants can be auto-generated (e.g., Halloween skin applied to best-performing asset)
- Fatigue detection window: performance typically declines after 3–5 days at scale — AI auto-rotates before the drop

#### AI creative production stack
- **UGC-style video generation**: AI produces lo-fi / "ugly ad" aesthetic videos at $7/video; 15 in under 1 hour
- **Moodboarding**: Tools like Mooed.ai and DALL-E suggest color palettes, visual themes, and asset concepts
- **Dubbing and localization**: Auto-generated voiceovers and subtitles for multilingual campaigns
- **Asset upscaling**: AI sharpens low-resolution assets for modern display resolutions across device tiers
- **Creative tagging**: Multimodal AI tags every visual, text snippet, and audio cue across all ad assets — surfaces which elements drive installs

#### NLP and player support chatbots
- In-game and support-channel bots deflect routine queries 24/7
- Bots use player history to personalize responses (strategy recommendations, targeted IAP offers)
- Continuously retrain on each conversation to improve accuracy

---

### 12.3 AI attribution stack (privacy-era standard)

The single-source MMP model is obsolete. The current best practice is a three-layer stack:

```
Layer 1 — Deterministic MTA
  └── MMP fingerprint matches, email-match, IDFA consented users (39% of iOS)

Layer 2 — Probabilistic modeling
  └── SKAN/AdAttributionKit postbacks + aggregated event data + modeled conversion values
  └── AI infers install source and predicted LTV from non-personal signals

Layer 3 — Marketing Mix Modeling (MMM)
  └── Statistical attribution of revenue across channels over time
  └── Fills gaps where neither deterministic nor probabilistic data is available
  └── Essential for long-term budget allocation and cross-channel ROAS modeling
```

**Key implication for skills**: Do not write UA measurement guidance that assumes clean user-level data from iOS. All iOS measurement must route through SKAN/AdAttributionKit probabilistic inference, with deterministic data as a supplement, not the default.

---

### 12.4 AI-powered retargeting and re-engagement

Skills covering retargeting or lapsed player recovery should include these AI-driven components:

#### Step 1 — AI segmentation
- Cluster lapsed players by behavior and value: "lapsed high spenders," "social casuals," "near-churn mid-payers"
- Feed session data, spend, level progress into ML audience builder
- Output: distinct cohorts for targeted creative and offer strategy

#### Step 2 — Churn prediction
- Train supervised ML model on historical player activity to churn
- Score active player base regularly on churn risk
- Trigger "rescue campaign" for high-risk players before they fully lapse: personalized push/email with free lives, special content, or discount
- Apply cool-down suppression for recently active or recently converted players (avoid ad fatigue)

#### Step 3 — Dynamic creative personalization
- Reference last played level, character, or store item in the re-engagement ad
- A/B test variations with AI guidance; auto-pause underperformers
- Frequency-cap intelligently: retarget quickly after a lull, suppress after a purchase window

#### Step 4 — Channel and timing optimization
- ML analyzes login patterns and adjusts bid timing so ads appear just before typical play sessions
- Multi-touch orchestration: push notification → paid social → in-app message reinforcement
- Budget shifts to best-performing channel in real time via DSP automation

#### Step 5 — Deep linking
- Every retargeting ad and message must deep-link to the exact game context (level, offer, store page)
- Deep-linked campaigns convert at ~3× generic links
- Test all links across device/OS permutations before launch

#### Measuring re-engagement lift (incrementality)
- Run holdout tests: AI predicts what a lapsed player would do without the ad — compare with the exposed group
- Measure true incrementality (causal campaign lift), not just "clicks came back"
- Label campaigns well so ML can identify which variants drive genuine conversion vs. natural return

---

### 12.5 AI in ad fraud detection

Ad fraud (bot clicks, fake installs, inflated bids) is a structural threat to UA efficiency. AI defends in three ways:

| Layer | What AI Does |
|-------|-------------|
| **Anomaly detection** | Flags abnormal click spikes from single IPs, install surges with no engagement |
| **Behavioral analysis** | Identifies device fingerprint clusters (classic fake-install signature) |
| **Real-time blocking** | Auto-filters fraudulent traffic before it counts toward CPI or ROAS |
| **Continuous retraining** | Each new fraud tactic encountered updates the model — adapts to emerging schemes |

**Tools in use**: Adjust Fraud Prevention Suite, AppsFlyer Protect360, CHEQ, TrafficGuard.

**Key implication**: CPI and ROAS figures from non-fraud-protected campaigns should be treated as inflated. Always validate MMP fraud filter settings before drawing performance conclusions.

---

### 12.6 AI creative velocity — operating model

Creative fatigue is now the primary performance constraint in mobile game UA, not budget or targeting. The AI-driven creative operating model:

```
Week 1-2:   Launch 3-5 creative concepts per format (video, playable, UGC-style, hybrid)
Day 3-5:    Fatigue signals appear → AI flags declining engagement per asset
Day 5-7:    AI rotates in fresh variants (swap hook, text overlay, cultural reference, character skin)
Weekly:     Human creative strategist reviews AI-surfaced winners → briefs next batch
Monthly:    Full concept refresh; AI moodboarding session for next themes
```

**Benchmark**: At scale, expect to rotate creatives every 5–10 days per audience segment. AI-generated UGC variants can extend refresh cycles by producing 15+ iterations in under 1 hour at ~$7 each.

---

### 12.7 AI skill quality checklist addendum (extends Section 11)

When reviewing any skill that touches UA, creative, or retargeting — add these AI-era checks:

- [ ] Acknowledges ML-powered bidding (Performance Max, Advantage+, or equivalent) as the baseline
- [ ] Does not treat manual bidding as the primary UA mechanism
- [ ] Includes creative fatigue monitoring and rotation cadence
- [ ] Addresses the three-layer attribution stack (deterministic + probabilistic + MMM)
- [ ] Retargeting guidance includes AI-based churn prediction and holdout testing for incrementality
- [ ] Fraud prevention is mentioned where campaign spend decisions are involved
- [ ] Does not assume clean iOS user-level data — models for 39% IDFA opt-in reality
