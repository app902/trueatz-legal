# TruEatz CHANGELOG

All notable changes to the TruEatz scoring algorithm and legal documents are tracked here. Public-facing for transparency and to demonstrate good-faith iteration.

---

## [v11.0] — May 3, 2026

### Legal
- Privacy Policy bumped to v11.0
- Terms of Service bumped to v11.0
- Effective and Last Updated dates moved to May 3, 2026
- No material changes to user rights, data handling, or contractual terms — version-tracking refresh only

### Algorithm
- No changes — algorithm remains at locked v1 ruleset (see entries below)

---

## [v10.0] — May 2, 2026

### Legal
- Full Privacy Policy and Terms of Service rewrite after 11 review passes each
- Plaintiff-lawyer attack vectors, regulator scrutiny, and international compliance pass (GDPR, CCPA, LGPD, PIPEDA, DPDP Act 2023, Australia Privacy Act 2025)
- App Store accountability laws addressed (Texas, Utah, Louisiana, California 2026)
- Google Play Health Apps Policy disclaimer added
- BIPA/CIPA/VPPA class-action carve-outs added
- Photos confirmed never leave device — on-device ML Kit OCR only
- Florida law jurisdiction with arbitration + 30-day opt-out
- Liability cap = greater of $50 or 12 months of subscription fees

---

## [v1.1.0] — May 2, 2026

### Algorithm — Tone audit
- 21 chemical entries softened in HARMFUL dictionary
- Replaced absolute language ("dangerous", "toxic", "causes") with research-grounded language ("associated with", "linked to", "may contribute to")
- Defamation defense hardening — no claims beyond what peer-reviewed citations support

---

## [v1.0.0] — May 1, 2026

### Algorithm — Founding version
- 0–100 scoring scale locked
- Sodium tiers (mg/100g): 0–150 / 150–400 / 150–700 / 700–1000 / 1000+ → 0/-5/-10/-15/-20 penalty
- Real-food modifier: ½ sodium penalty when ingredients ≤3, all recognizable foods, no nitrites/phosphates/added sugar/natural flavors
- Fermented bonus: +5 (does NOT exempt sodium penalty)
- Condiment modifier: ⅓ sodium penalty
- Ingredient count penalty: 5–10 (-2), 10–20 (-5), 20+ (-10)
- Beverage liquid sugar multiplier: ×1.2
- Carcinogen cap: any IARC Group 1 ingredient → score capped at 35
- Real-food bonus: 90%+ recognizable ingredients → +10
- Whitelisted additives (no penalty): calcium lactate, xanthan gum, guar gum, lactic/citric/ascorbic acid, pectin, agar
- 64+ chemical entries with peer-reviewed study citations

---

## Philosophy notes

TruEatz scoring rejects outdated Nutri-Score dogma. Saturated fat from real meat, calorie density, and natural sodium are not penalized. Chemical additives, nitrites, seed oils, refined sugar, and ultra-processed foods are.

This CHANGELOG is public so users, brands, and regulators can audit every scoring rule change with date and rationale. Brands cannot pay to influence scores. TruEatz has no advertising, no affiliate deals, and no commercial relationships with food manufacturers.

For questions: **app@trueatzapp.com**
