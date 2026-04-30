# Game Marketing Skills — TODO

*Updated: 2026-04-30*

## Current Status
Phase 1 complete: `game-marketing-context` skill built, tested, and eval'd.
`KNOWLEDGE.md` extended with Section 11 (Skill Qualification Protocol, pass/fail gates, scoring rubric, contributor template, calibration examples) and expanded glossary (20 new terms from Adjust guides).
`KNOWLEDGE.md` further extended with Section 12 (AI-Powered Tools in Mobile Game Marketing) and 15 new glossary terms from Segwise.ai 2024–2025 data — covers AI benchmarks, ML bidding platforms, DCO, creative velocity, the three-layer attribution stack, AI retargeting workflow, fraud detection, and a Section 12.7 AI-era skill quality addendum.

---

## Iteration 2 — Fix `game-marketing-context` before moving on

Issues found during eval that must be addressed:

- [ ] Fix stale UA channel names: `IronSource` → `Unity LevelPlay`, `Vungle` → `Liftoff Monetize`
- [ ] Add soft launch market rationale (why CA/AU/NZ: English-speaking, similar CPI to US, GDPR-light = cheap validated data before Tier 1 spend)
- [ ] Add core loop articulation template — skill calls it "most critical field" but gives no scaffolding
- [ ] Add genre-based CPI/retention benchmark ranges (hyper-casual D1 ~50%, casual D1 ~35–40%, mid-core D1 ~25–30% etc.)
- [ ] Sharpen eval assertions to be discriminating — current assertions pass with or without the skill; test for skill-specific terminology (genre taxonomy labels, `[NEEDS INPUT]` discipline, launch phase table format)

---

## Roadmap

### Phase 1 — Foundation ✅
| # | Skill | Status |
|---|-------|--------|
| 1 | `game-marketing-context` | ✅ Built & eval'd (iteration 1) |

### Phase 2 — New Skills
| # | Skill | Status |
|---|-------|--------|
| 2 | `game-launch` | ⏳ Next |
| 3 | `ua-strategy` | ⏳ Pending |
| 4 | `player-targeting` | ⏳ Pending — find & target ideal players (UA segments, lookalikes, competitor audiences, creator seeding) |
| 5 | `store-creative` | ⏳ Pending |
| 6 | `live-ops` | ⏳ Pending |

### Phase 3 — Update Existing Skills
| # | Skill | Status |
|---|-------|--------|
| 7 | `aso-audit` | ⏳ Pending — add game-specific scoring, remove SaaS framing |
| 8 | `paid-ads` | ⏳ Pending — replace B2B with game UA networks + CPI/ROAS metrics |
| 9 | `ad-creative` | ⏳ Pending — gameplay video, playables, TikTok gaming formats |
| 10 | `analytics-tracking` | ⏳ Pending — D1/D7/D30 retention, ARPPU, ARPDAU, LTV |
| 11 | `pricing-strategy` | ⏳ Pending — IAP design, starter packs, whale funnels, battle pass |
| 12 | `churn-prevention` | ⏳ Pending — lapsed player reactivation, win-back campaigns |
| 13 | `social-content` | ⏳ Pending — TikTok gaming, YouTube Shorts, Discord |
| 14 | `community-marketing` | ⏳ Pending — Discord strategy, Reddit gaming, creator seeding |

### Phase 4 — Archive SaaS-Only Skills ✅
| Skills moved to `skills/legacy-saas` | Status |
|--------------------------------------|--------|
| `cold-email`, `revops`, `sales-enablement`, `competitor-alternatives`, `directory-submissions`, `programmatic-seo`, `schema-markup`, `site-architecture`, `lead-magnets`, `free-tool-strategy`, `video`, `form-cro`, `popup-cro`, `signup-flow-cro`, `onboarding-cro`, `page-cro`, `copywriting`, `copy-editing`, `email-sequence`, `ai-seo`, `seo-audit`, `competitor-profiling` | ✅ Moved |

---

## Notes
- Skills must stay cross-agent compatible (no Claude Code-specific syntax in SKILL.md)
- All skills must pass validate-skills.sh before merging
- Featured game for testing: [LUTA: Luminoria Tactics](https://play.google.com/store/apps/details?id=com.HonStudios.LuminoriaTactics)
