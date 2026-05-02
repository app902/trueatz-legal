# TruEatz Scoring Algorithm Changelog

All notable changes to the TruEatz food scoring algorithm, chemicals dictionary, and risk classifications are documented in this file.

This changelog exists for **transparency, accountability, and good-faith documentation**. Every scoring decision is traceable to a published date, a peer-reviewed source or regulatory authority, and a documented rationale.

The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) and adheres to [Semantic Versioning](https://semver.org/) where applicable to scoring rules.

**Versioning convention:**
- **MAJOR** (X.0.0) — fundamental scoring philosophy change (e.g., switching from Nutri-Score to paleo-aligned)
- **MINOR** (1.X.0) — adding/removing chemicals, adjusting risk levels, adding penalty/bonus categories
- **PATCH** (1.0.X) — wording updates, tone changes, citation additions, typo fixes

---

## [Unreleased]

Tracking decisions in progress, not yet shipped.

---

## [1.1.0] — 2026-05-02

### Changed — Tone audit on chemical descriptions

Comprehensive review of language in `HARMFUL` dictionary to replace categorical claims with evidence-hedged language. Same warning intent, same scientific accuracy, but reframed as opinion-based assessment rather than absolute fact. **Rationale:** First Amendment opinion protection requires that scoring claims be framed as analysis based on disclosed sources, not categorical statements.

**21 entries softened:**

| Ingredient | Before | After |
|---|---|---|
| Yellow 5 | "Causes hyperactivity" | "Research has linked artificial dyes to hyperactivity in some children" |
| Tartrazine | "genotoxic" | "genotoxicity findings" |
| Blue 2 | "Animal studies showed" | "Some animal studies have observed" |
| HFCS | "bypasses normal metabolism" | "metabolized differently than other sugars" |
| Sucralose | "is genotoxic and causes" | "may be genotoxic and may contribute to" |
| Saccharin | "Caused bladder cancer in rats" | "Linked to bladder cancer in rat studies" |
| BHT | "Disrupts endocrine system" | "Studies suggest endocrine-disrupting effects" |
| Sodium benzoate | "forms benzene" | "can form benzene" |
| MSG | "Triggers headaches" | "May trigger headaches, flushing, or palpitations" |
| Carrageenan | "Triggers gut inflammation" | "Research has linked to gut inflammation" |
| Polysorbate 80 | "Disrupts the gut microbiome" | "Studies suggest possible disruption of" |
| Carboxymethylcellulose | "Damages gut lining" + "studies confirm" | "Linked to gut lining changes" + "studies have observed" |
| Calcium disodium EDTA | "Strips minerals from body" | "May bind minerals in body" |
| Dextrose | "Causes rapid blood sugar spikes" | "Linked to rapid blood sugar spikes" |
| Modified corn starch | "blood sugar spike" | "may spike blood sugar" |
| Soybean oil | "drives inflammation" | "may contribute to inflammation per recent research" |
| Cottonseed oil | "often heavy pesticide residues" | "may carry pesticide residues" |
| Sunflower oil | "that oxidizes" | "that can oxidize" |
| Partially hydrogenated | "Strongly linked" | "Linked to" |
| Yellow 6 | "a known carcinogen" | "classified as a known carcinogen by IARC" |
| TBHQ | "Animal studies showed" | "Some animal studies have observed" |
| Azodicarbonamide | "potential carcinogens" | "classified as possible carcinogens" |
| DATEM | "Heart muscle damage" | "Heart muscle changes in animal studies" |
| Sodium aluminum phosphate | "linked to brain disease" | "studied for possible links to neurodegenerative conditions" |

**Preserved as-is (already legally safe):**
- Direct regulator quotes ("WHO/IARC Group 2B," "Listed by California as a known carcinogen," "Banned in EU since 2022")
- Direct chemistry statements ("Forms nitrosamines" — basic chemistry)
- Citations to NTP, IARC, EFSA, FDA reports

---

## [1.0.0] — 2026-05-01 — Founding scoring philosophy locked

Initial public version. All decisions below documented as the founding philosophy of TruEatz scoring. **Rationale: paleo-aligned, real-food-focused, evidence-based.**

### Scoring formula

Base score: 100 points. Penalties subtract; bonuses add. Final score is 0–100 inclusive.

### Sodium rules — locked

Decision: **Do not penalize sodium for most users.** Threshold-based approach only.

- < 0.4 g sodium / 100 g — **No penalty**
- 0.4 – 1.5 g / 100 g — **No penalty (normal range)**
- 1.5 – 2.5 g / 100 g — **Advisory tag, no point penalty (yellow tier)**
- > 2.5 g / 100 g — **−10 penalty** (only for ultra-processed foods)
- **Fermented foods** (kimchi, sauerkraut, miso, kombucha, pickles, kefir, yogurt, soy sauce, fish sauce) — **EXEMPT from sodium penalty**, gain probiotic note

**Citations supporting:**
- Mente et al. 2018 (PURE study) — *Lancet* — low-salt diets do not clearly benefit most people
- Graudal et al. 2020 — Cochrane Database — meta-analysis on sodium intake and mortality
- He & MacGregor 2009 — *Cochrane Database* — population-level salt reduction effects

### Saturated fat — NO penalty

Decision: **Do not penalize saturated fat in unprocessed foods.**

**Rationale:** The 1980s saturated fat hypothesis has been substantially weakened by modern meta-analyses.

**Citations:**
- Siri-Tarino et al. 2010 — *Am J Clin Nutr* — meta-analysis of 347,747 subjects found no significant association between saturated fat and CVD
- Chowdhury et al. 2014 — *Annals of Internal Medicine* — systematic review of 72 studies
- Astrup et al. 2020 — *J Am Coll Cardiol* — saturated fat and CVD reassessment

### Seed oils flagged HIGH risk

Decision: **Industrial seed oils (soybean, canola, corn, cottonseed, sunflower, safflower, grapeseed) flagged as high risk.**

**Citations:**
- DiNicolantonio & O'Keefe 2018 — *BMJ Open Heart* — omega-6 oxidized linoleic acid metabolites
- Ramsden et al. 2016 — *BMJ* — Sydney Diet Heart Study reanalysis (overturned earlier findings)

### Sugar penalty rules

- < 1 g / 100 g — **No penalty**
- 1 – 5 g / 100 g — **Advisory (yellow tier), no points off**
- > 5 g / 100 g — **−10 penalty**
- > 15 g / 100 g — **−20 penalty (severe)**
- Whole-fruit / dairy lactose / vegetable sugars — **EXEMPT** when they're the natural source

**Citations:**
- Stanhope et al. 2009 — *J Clin Invest* — fructose and metabolic dysfunction
- Lustig 2010 — fructose and metabolic syndrome
- Yang et al. 2014 — *JAMA Intern Med* — added sugar intake and CVD mortality

### Real food bonus — +10

Decision: **Products with 90%+ recognizable whole-food ingredients receive a +10 bonus.**

**Rationale:** Reward minimally processed foods explicitly. Aligns with Monteiro NOVA classification of unprocessed/minimally processed (NOVA Group 1).

**Citations:**
- Monteiro et al. 2019 — *Public Health Nutrition* — NOVA classification
- Hall et al. 2019 — *Cell Metabolism* — ultra-processed food and ad libitum intake (NIH NIDDK study)

### Whitelist — additives that DO NOT trigger penalty

**Rationale:** These are either naturally occurring, food-grade, or have strong safety profiles. Penalizing them would cause false negatives on otherwise clean products.

| Additive | Reason |
|---|---|
| Calcium lactate | Calcium salt of lactic acid — naturally found in fermented foods |
| Xanthan gum | Fermentation-derived polysaccharide — safe at typical food levels |
| Guar gum | Plant-derived (guar bean) soluble fiber |
| Lactic acid | Naturally occurring in fermented foods |
| Citric acid | Naturally occurring (citrus, fermentation) |
| Ascorbic acid | Vitamin C |
| Pectin | Naturally occurring fiber from fruit cell walls |
| Agar | Seaweed-derived |

### HARMFUL dictionary — initial chemicals tracked (64+)

Categories of additives flagged in v1.0.0 with peer-reviewed and/or regulator citations:

- **Artificial colors** — Red 40, Yellow 5, Yellow 6, Blue 1, Blue 2, Tartrazine
- **Artificial sweeteners** — Aspartame, Sucralose, Acesulfame Potassium, Saccharin
- **Sweeteners (other)** — HFCS, Corn syrup, Maltodextrin, Dextrose, Modified corn starch
- **Preservatives** — Sodium nitrite, Sodium nitrate, BHA, BHT, Sodium benzoate, Potassium benzoate, TBHQ, Propyl gallate, Calcium disodium EDTA, Calcium propionate
- **Colorings** — Caramel color (Class III/IV), Titanium dioxide, Carmine, Annatto
- **Flavor enhancers** — MSG, Hydrolyzed vegetable protein, Autolyzed yeast, Disodium inosinate, Disodium guanylate
- **Dough conditioners** — Potassium bromate, Azodicarbonamide, Calcium peroxide, Sodium stearoyl lactylate, L-cysteine
- **Trans fats** — Partially hydrogenated oils, Monoglycerides (loophole), Diglycerides (loophole)
- **Thickeners/Emulsifiers** — Carrageenan, Polysorbate 60, Polysorbate 80, Carboxymethylcellulose, DATEM
- **Phosphates** — Sodium phosphate, Sodium tripolyphosphate, Phosphoric acid
- **Industrial seed oils** — Soybean, Canola, Vegetable, Sunflower, Safflower, Corn, Cottonseed, Grapeseed, Rice bran
- **Refined grains** — Enriched flour, Enriched wheat flour, Bleached flour
- **Solvents** — Propylene glycol
- **Aluminum** — Sodium aluminum phosphate
- **Vague/loophole** — Natural flavors (FDA GRAS loophole), Artificial flavors

### Risk levels defined

- **Low (🟡 yellow dot)** — Mild concern, generally safe in moderation
- **Medium (⚠️ yellow/orange)** — Research suggests caution; emerging or animal-study evidence
- **High (🚨 red)** — Strong evidence of harm OR banned in major jurisdictions OR classified by IARC/NTP

### Auth & community rules — locked

- Sign-in required for full features
- Anonymous handle by default; custom username changeable 1× per month
- Report Issue: +10 pts (1 per barcode per 24 hours)
- Upvotes: +1 pt per upvote, max +20
- 3+ upvotes auto-approves a submission
- 3+ downvotes sends to dev queue
- Points Bank: linear ~833 pts = 1 month Premium; no cap; no expiration
- 10,000 pts = Crown badge + 1 year Premium banked

---

## Pre-1.0.0 — Development phase (2026-04 and earlier)

Internal development. No public users. Not version-tracked.

Major design decisions made during this phase (now locked in 1.0.0 above):
- Switch from Nutri-Score base to paleo-aligned scoring philosophy
- Removal of saturated fat penalty (originally inherited from Nutri-Score logic)
- Real food bonus introduction
- Sodium threshold relaxation
- Fermented food exemption logic

---

## How to use this changelog

### For users
This document is publicly available so you can see exactly when and why TruEatz scoring rules change. Every decision is sourced. We do not make secret algorithm tweaks.

### For brands
If a TruEatz score for your product changes, you can trace exactly when and why by looking at the version history. If you believe a scoring rule is incorrect or your product has been mis-scored, contact app@trueatzapp.com — we review all good-faith concerns.

### For researchers / press
Citations for every rule are listed. We welcome scrutiny. If you find a rule that should be updated based on newer evidence, send the citation to app@trueatzapp.com with subject "Scoring Update."

### For TruEatz team — adding new entries

New entries should be added at the top under `[Unreleased]` and moved to a numbered version when shipped. Use this format:

```
## [Version] — YYYY-MM-DD

### Added
- New chemical/rule/feature with citation

### Changed
- Existing rule modification with rationale + citation

### Removed
- Removed chemical/rule with rationale

### Fixed
- Bug fix or data correction
```

Each entry must include at least one of:
1. Peer-reviewed citation (PubMed-indexed preferred)
2. Regulatory citation (FDA, EFSA, IARC, WHO, NTP, state law)
3. Documented rationale tied to existing scoring philosophy

**Do not add scoring rules without citations.** That's the whole point of this document.

---

*TruEatz — Real food. Real science. Documented decisions.*

*This changelog is part of TruEatz's commitment to transparency under the Independence Statement at trueatzapp.com/independence.*
