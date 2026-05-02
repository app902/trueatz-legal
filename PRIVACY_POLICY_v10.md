# TruEatz Privacy Policy

**Effective Date:** May 2, 2026
**Last Updated:** May 2, 2026
**Version:** 10.0

TruEatz is built on a simple promise: **we collect the minimum amount of data needed to make the App work, and we never sell it to anyone.** This document explains exactly what we collect, why, your choices, and your rights.

If you have questions, email us at **app@trueatzapp.com**.

This Policy is incorporated by reference into our Terms of Service.

---

## 1. Who We Are

TruEatz ("we," "us," "our," the "Company") is the operator of the TruEatz mobile application (the "App") and the website at trueatzapp.com (together, the "Service").

**Contact:**
- Email: app@trueatzapp.com
- Country of operation: Florida, United States

For users in the European Economic Area (EEA) or United Kingdom, TruEatz is the data controller for personal data described in this Policy. We do not currently appoint a designated EU representative under GDPR Article 27 because our processing of EEA/UK personal data is occasional, low-risk, and not large-scale. We do not require a Data Protection Officer under GDPR Article 37 because our processing does not involve large-scale systematic monitoring or large-scale processing of special category data. We will appoint a representative or DPO if our processing scope changes and update this Policy accordingly.

Section headings in this Policy are for convenience only and do not affect interpretation.

---

## 2. What We Collect

### 2.1 Account information (required to use the App)

- **Email address** — to create your account, send verification, password resets, and required service communications
- **Display name** (optional) — what you choose to show publicly
- **Anonymous username** — auto-generated when you sign up; you may change it once per month
- **Password** — stored only as a one-way hash; we never see your plaintext password

We do **NOT** collect: real name, date of birth, phone number, address, gender, ethnicity, income, religion, political views, sexual orientation, biometric identifiers, or any government identifiers.

### 2.2 App activity (stored locally and in our cloud)

- **Scan history** — products you've scanned (barcode + result)
- **Points earned** — your contribution count and level
- **Submissions** — products, ingredient lists, store information, and reports you submit
- **OCR-extracted text** — text our software reads from product labels you photograph (see Section 2.5)

### 2.3 Device & technical information (limited)

- **Device type and OS version** — to debug crashes and improve compatibility
- **App version** — to roll out updates safely
- **Crash logs** — automatically generated when the App encounters an error, processed by **Firebase Crashlytics** (Google). Stack traces, device model, and OS version only — never personal content from your scans, submissions, or account. Used solely for debugging and product stability — never for advertising, profiling, or behavioral analytics.
- **Push notification tokens** — a unique device-specific token used only to deliver notifications you've opted into

### 2.4 Subscription & payment data (Premium only)

When you purchase a Premium subscription, **Apple App Store or Google Play Store handles the entire transaction**. We never see, receive, or store your full payment card details, billing address, or payment processor account.

We receive only:
- Your subscription status (active / cancelled / expired / refunded)
- The subscription tier you purchased
- A receipt token to verify your subscription with the store

### 2.5 Photos and biometric data — what we do and don't do

The App requires camera access to scan barcodes and product labels. There are three distinct ways images are handled, and we want to be explicit about all three:

**(a) Barcode scans** — processed entirely on your device. We extract only the numeric barcode value. The image is never uploaded.

**(b) Label OCR (text recognition)** — processed entirely on your device using **Google ML Kit's on-device text recognition library**. The OCR photo never leaves your device. Only the extracted text is uploaded to our database. After OCR processing, image data is discarded from device memory.

**(c) User-attached product photos (optional, only when you choose)** — when you tap "+ Submit Product" and explicitly attach a photo of a product (front-of-package image, label photo, etc.), that photo IS uploaded to our database (Firebase Cloud Storage) and may be displayed publicly to other users alongside the product entry. **You decide what to upload and what's in the photo.**

**Across all three image types:**

We do **NOT** extract, generate, store, or analyze biometric identifiers of any kind, including face geometry, facial recognition templates, fingerprint patterns, iris scans, retina scans, voiceprints, hand geometry, or palm geometry.

We do **NOT** detect, identify, recognize, or track individual people in photos. We do not run face detection, person recognition, gait analysis, or any biometric processing on any image.

**We have designed the App to avoid collecting biometric identifiers as defined by the Illinois Biometric Information Privacy Act (BIPA), Texas Capture or Use of Biometric Identifier Act (CUBI), Washington's biometric statute, and comparable laws.**

If you submit a photo (option c above) that incidentally contains a person — for example, your hand holding a product — please be aware that photo will be publicly visible in the food database. We recommend cropping out hands, faces, or any identifying information before submitting.

### 2.6 What we never collect

- Your real name
- Your home, work, or shipping address
- Your phone number
- Your social security number, driver's license, passport, or any government ID
- Your payment information beyond what your app store handles
- Your contacts, microphone audio, or files outside the App
- Your precise GPS location or coarse location
- Your browsing history outside the App
- Your photos other than those you explicitly capture or attach for the App's stated purpose
- Special category data under GDPR (race, ethnicity, religion, political views, sex life, sexual orientation, biometric data, health data, genetic data, trade union membership)

---

## 3. App Permissions

The App requests these device permissions:

| Permission | Why we need it | Required? |
|---|---|---|
| Camera | Scan barcodes and read product labels | Required for core function |
| Notifications | Send recall alerts and achievements (if you opt in) | Optional — App works without it |
| Photo library / files | Only if you choose to attach a photo via "+ Submit Product" | Optional — App works without it |

We do **NOT** request: location, contacts, microphone, calendar, motion data, background activity, health data, or any other device permissions.

You can revoke any permission at any time through your device's settings.

---

## 4. How We Use Your Data

We use the data above only for these purposes:

1. **To run the App** — sign you in, save your scans, sync points across devices, deliver Premium features
2. **To improve the food database** — your submissions and OCR-extracted text help fill in missing products for the community
3. **To send transactional emails** (always on while account is active) — verification, password reset, security alerts, account closure confirmations, subscription receipts and renewal warnings, material changes to this Policy or our Terms, service availability or downtime notices. **Transactional emails are not marketing emails** and cannot be unsubscribed from individually while your account is active.
4. **To send optional push notifications** — see Section 6
5. **To debug and improve the App** — fix crashes, optimize performance, identify bugs
6. **To enforce our rules** — flag spam, abusive submissions, fraud, or violations of our Terms
7. **To verify your subscription** — confirm Premium status with Apple or Google
8. **To comply with legal obligations** — respond to valid court orders, subpoenas, or law enforcement requests as required by law

We do **NOT** use your data for:
- Targeted or behavioral advertising
- Selling to data brokers or third parties
- Building shadow profiles
- Training AI or machine learning models on your personal information
- Marketing emails or promotional drip campaigns (see Section 6.3)
- Profiling for solely automated decisions that produce legal effects

---

## 5. Who We Share Data With

We share **only** what's necessary, and **only** with these categories of trusted partners:

- **Firebase / Google Cloud (Google LLC)** — our authentication, database, file storage, push notification, and crash reporting backend; stores your account info, scans, submissions, attached photos, and crash logs. Google's processing is governed by their Data Processing Addendum: cloud.google.com/terms/data-processing-addendum
- **Apple App Store / Google Play Store** — handle App installation, subscriptions, and any in-app purchases (we never see your full payment details)
- **Open Food Facts (open-source food database)** — when we fetch product information, we send only the barcode, never your identity or any account data. Open Food Facts may log API requests according to their own privacy policy at openfoodfacts.org/privacy.

Data shared with our service providers (Firebase, Apple, Google) is **not a "sale" or "sharing" under CCPA / CPRA** because these providers are bound by written contracts that prohibit them from using the data for their own commercial purposes outside of providing contracted services.

We do **NOT** share your data with:
- Advertising networks (we use no ad SDKs)
- Data brokers
- Marketing partners or affiliate networks
- Government agencies (except when legally required by valid court order, subpoena, or law)
- AI / ML model training providers
- Credit bureaus or fraud-scoring services
- Insurance companies, employers, or background-check providers

### 5.1 Legal disclosures

We may disclose personal information when we believe in good faith that disclosure is required to:
- Comply with a valid legal process (subpoena, court order, warrant)
- Enforce our Terms of Service
- Protect the rights, property, or safety of TruEatz, our users, or the public
- Detect or prevent fraud, security threats, or technical issues

When legally permitted, we will notify the affected user before disclosure.

### 5.2 Business transfers

If TruEatz is involved in a merger, acquisition, financing, reorganization, bankruptcy, or sale of assets, your information may be transferred as part of the transaction. The acquiring entity will be bound by this Policy or will provide notice and the opportunity to opt out before applying any new policy.

---

## 6. Notifications and Communications

### 6.1 Transactional emails (always on while account is active)

Required for the App to function:
- Email address verification
- Password reset links
- Security alerts (suspicious sign-in attempts)
- Account closure confirmations
- Subscription receipts, renewal warnings, refund confirmations
- Material changes to this Policy or our Terms of Service
- Service availability, downtime, or breach notices

**Transactional emails are not marketing emails.** They cannot be unsubscribed from individually while your account is active. To stop receiving them entirely, delete your account.

### 6.2 Push notifications (opt-in, can be disabled at any time)

If you grant push notification permission, we may send you:
- **Recall alerts** (Premium feature) — when a product you've scanned is recalled by the FDA or manufacturer. **We do not guarantee delivery, timeliness, or completeness of recall notifications.** Always check official FDA recall sources directly when safety is critical.
- **Achievement notifications** — when you unlock a new level, badge, or Crown
- **Community activity** (optional, off by default) — when one of your submissions is approved or upvoted

Disable any of these in your device's notification settings:
- iOS: Settings → Notifications → TruEatz
- Android: Settings → Apps → TruEatz → Notifications

A future App version will add in-App granular notification toggles by category.

### 6.3 Marketing communications

**As of May 2, 2026, TruEatz has never sent marketing or promotional emails or push notifications**, and has not done so in the preceding 12 months. We do not maintain a marketing mailing list.

If we ever introduce optional marketing communications, we will:
- Update this Policy first (with at least 30 days' advance notice)
- Make them strictly opt-in (you must affirmatively agree)
- Provide a one-click unsubscribe in every message
- Respect opt-out signals immediately

---

## 7. Public vs. Private Information

Some things you do in TruEatz are visible to other users:

**PUBLIC** (visible to other users):
- Display name and anonymous username
- Level (Sprout, Foodie, Health Hunter, Food Guardian, Champion, Crown holder) and points total
- Submissions to the public food database (ingredient lists, store information, OCR-extracted text, attached photos)
- Reports you file on existing products
- Upvotes and downvotes you cast

**PRIVATE** (visible only to you):
- Email address
- Scan history
- Manual entries you type (these never leave your device)
- "Blacklist" or custom avoid lists (Premium feature)
- Crash logs
- Subscription status
- Any data tied to your account that is not explicitly listed as Public

If you don't want a submission, photo, or attribution to be public, **don't submit it**.

---

## 8. Children's Privacy and Age Verification

### 8.1 General age requirement

TruEatz is not intended for users under 13. We do not knowingly collect personal data from children under 13. If we learn we have, we will delete it within 7 days.

### 8.2 App Store Accountability Laws (Texas, Utah, Louisiana, California, 2026)

Several U.S. states have enacted "App Store Accountability" laws taking effect in 2026 that require app stores to share certain age signals with developers. Where these laws apply:

- We may receive an **age category** signal from Apple App Store or Google Play Store (e.g., "under 13," "13–15," "16–17," "18+") when you install or use the App in those states
- We use this signal **solely for age-gating purposes** — to enforce our 13+ minimum age requirement and apply any required parental consent flows
- We **do not** retain, share, sell, or use this age signal for any other purpose
- We delete the signal from our systems once age verification is complete, as required by Texas law
- For users under 18, we will rely on app store verification of parental consent before enforcing any contract terms against the user, as required by these laws
- Users 13–17 should review these Terms with a parent or guardian

### 8.3 COPPA compliance and parental email

We comply with the U.S. Children's Online Privacy Protection Act (COPPA). We do not knowingly market to or collect personal information from children under 13.

**If you are a parent who used your own email to create an account on behalf of a child under 13, please contact us immediately at app@trueatzapp.com.** We will delete the account and all associated data within 7 days. Parental email addresses associated with under-13 accounts will also be removed.

If you are a parent and discover your child has independently created an account, email app@trueatzapp.com and we will delete the account and data within 7 days.

---

## 9. Your Rights

You have the right to:

- **Access** your data — view what we have on you
- **Correct** inaccurate data — change your display name, username, email
- **Delete** your account and all associated data
- **Export** a copy of your data in a portable format
- **Object** to processing for any reason
- **Withdraw consent** to optional data uses
- **Opt out** of any sharing or sale of your personal information (we don't sell or share, but the opt-out exists)
- **Lodge a complaint** with a regulator (see below)

To exercise any of these rights, go to the **About** tab → tap your **Profile** → use **Sign Out**, **Delete Account**, or email app@trueatzapp.com.

If you delete your account:
- Your email, scan history, and personal data are permanently removed within 30 days
- Submissions you made to the public food database will be **pseudonymized** — your username is replaced with a generic label such as "Anonymous Contributor" and any link to your account is severed. The submission data itself (ingredient lists, photos you submitted) may continue to be displayed publicly because it is part of the shared community database.
- Backup copies are purged within 90 days

We respond to all rights requests within 30 days (45 days for CCPA / California requests where allowed by law).

### 9.1 California (CCPA / CPRA)

California residents have additional rights:
- The right to know what personal information we collect
- The right to delete personal information
- The right to correct inaccurate information
- The right to opt out of "sale" or "sharing" of personal information
- The right to limit use of sensitive personal information
- The right to non-discrimination for exercising these rights

**As of May 2, 2026, TruEatz has never sold or shared personal information** as defined by the California Consumer Privacy Act (CCPA) and California Privacy Rights Act (CPRA), and has not sold or shared personal information in the preceding 12 months.

Because we do not sell or share personal information, we are not required to display a "Do Not Sell or Share My Personal Information" link. However, you may email app@trueatzapp.com with subject "California Privacy Request" to receive written confirmation of our non-sale status or exercise other CCPA / CPRA rights.

You may designate an authorized agent to make a request on your behalf, subject to our verification of the agent's authority and your identity.

We honor the **Global Privacy Control (GPC)** browser signal where applicable.

### 9.2 European Economic Area / United Kingdom (GDPR / UK GDPR)

EEA and UK residents have rights including access, rectification, erasure, restriction, data portability, and objection. The legal basis for our processing:

- **Contract** (Art. 6(1)(b)) — to provide the App you signed up for
- **Legitimate interest** (Art. 6(1)(f)) — to improve the App, prevent fraud, secure the Service
- **Consent** (Art. 6(1)(a)) — for any optional features (you can withdraw at any time)
- **Legal obligation** (Art. 6(1)(c)) — to comply with applicable laws

For UK users, we rely on the UK International Data Transfer Agreement (IDTA) or the UK Addendum to EU Standard Contractual Clauses for transfers to the United States.

To file a complaint, contact your local data protection authority or email us first at app@trueatzapp.com. UK users may contact the Information Commissioner's Office (ICO) at ico.org.uk.

### 9.3 Other U.S. states

Residents of Virginia (VCDPA), Colorado (CPA), Connecticut (CTDPA), Utah (UCPA), Texas (TDPSA), Oregon (OCPA), Montana (MCDPA), and other states with comprehensive privacy laws have similar rights to access, delete, correct, and opt out of targeted advertising or profiling. Email app@trueatzapp.com to exercise your rights.

All US users may also file complaints with the **Federal Trade Commission** at ftc.gov/complaint.

### 9.4 Other international users

- **Australian residents** have rights under the Privacy Act 1988 (Cth) and may complain to the Office of the Australian Information Commissioner (OAIC).
- **Canadian residents** have rights under PIPEDA and may complain to the Office of the Privacy Commissioner of Canada.
- **Brazilian residents** have rights under the LGPD and may complain to the ANPD.
- **Indian residents** have rights under the DPDP Act 2023 and may complain to the Data Protection Board of India once established.

We process such requests under the same procedures described above.

---

## 10. Data Retention

| Data type | Retention |
|---|---|
| Account data (email, display name, username) | Active life of account; deleted within 30 days of account closure |
| Scan history | Active life of account; deleted with account |
| OCR-extracted text (in cloud database) | Indefinitely (pseudonymized after account deletion) |
| User-attached product photos (Firebase Storage) | Indefinitely (pseudonymized after account deletion) |
| OCR original photos | Never stored — discarded from device memory after on-device processing |
| Crash logs | 90 days, then deleted |
| Push notification tokens | Refreshed by device; deleted with account |
| Submissions to public food database | Indefinitely (pseudonymized after account deletion) |
| Subscription receipts | 4 years (US tax / consumer protection statutes of limitations) |
| Backup copies | Purged within 90 days of primary deletion |
| Age verification signals (where collected) | Deleted upon completion of verification |
| Correspondence with our support / privacy team | 2 years |

---

## 11. Security and Account Responsibility

### 11.1 How we protect your data

We protect your data using:
- TLS 1.2+ encryption for all data in transit
- Encryption at rest in Firebase
- Email + password authentication with required email verification
- Rate limiting and abuse detection
- Limited employee access to production systems on a need-to-know basis
- Regular review of access logs and dependencies

### 11.2 Your responsibility

**You are responsible for keeping your password confidential and your account secure.** Notify us immediately at app@trueatzapp.com if you suspect unauthorized access to your account.

**We are not liable for losses, charges, submissions, content, or other consequences resulting from your failure to maintain account security or from your sharing of credentials with others**, except as required by applicable law.

### 11.3 Breach notification

**No system is 100% secure.** If we discover a breach affecting your data, we will:
- Notify affected users without undue delay
- Notify within 72 hours of discovery where required by GDPR or applicable state breach notification laws
- Report to relevant authorities as required by law
- Provide information about the breach, the data affected, and recommended steps

To report a security vulnerability, suspected breach, or unauthorized account access, email app@trueatzapp.com with subject "Security."

---

## 12. International Data Transfers

TruEatz is operated from the United States. If you use the App from outside the US, your personal data may be transferred to and processed in the US.

For transfers from the EEA to the US, we rely on:
- The European Commission's Standard Contractual Clauses (SCCs)
- Firebase's existing SCCs with Google Cloud as our infrastructure provider

For transfers from the UK to the US, we rely on:
- The UK International Data Transfer Agreement (IDTA), or
- The UK Addendum to the EU Standard Contractual Clauses

For transfers from Switzerland, we rely on the Swiss Federal Data Protection and Information Commissioner's recognized SCC mechanism.

By using the App from outside the US, you acknowledge this transfer.

---

## 13. Third-Party Services and SDKs

The App contains **no advertising SDKs, no third-party analytics SDKs, and no marketing trackers**. Our complete list of third-party services:

| Service | Purpose | Data shared |
|---|---|---|
| Firebase Authentication (Google) | User sign-in & verification | Email, password hash, device token |
| Firebase Firestore (Google) | Database | Account, scans, submissions |
| Firebase Cloud Storage (Google) | File storage for product images you choose to submit | Submitted images only |
| Firebase Cloud Messaging (Google) | Push notifications | Device push token |
| Firebase Crashlytics (Google) | Crash reporting | Anonymous stack traces, device model, OS version |
| Google ML Kit Text Recognition (on-device) | Reading text from photos | None — runs entirely on your device |
| Apple App Store / Google Play Store | App distribution & in-app purchases | Subscription status, receipt token |
| Open Food Facts API | Public food database lookups | Barcode only |

Each service has its own privacy policy. Our use of Google Firebase services is governed by Google's Data Processing Addendum.

If we add or remove third-party services in a way that materially changes how your data is processed, we will update this Policy and notify you under Section 16.

---

## 14. Cookies and Website

The TruEatz mobile App does not use cookies (cookies are a web browser concept).

The trueatzapp.com **website** is currently a placeholder marketing site with no analytics, no third-party trackers, and no advertising cookies. If we expand the website to include analytics, login, interactive features, or any cookie-using functionality, we will:

- Update this Policy first
- Post a cookie banner with consent options where required
- Respect "Do Not Track" and Global Privacy Control (GPC) browser signals
- Disclose the specific cookies in use, their purpose, retention, and recipients

---

## 15. Health App Disclaimer (Google Play Health Apps Policy)

TruEatz provides educational information about packaged foods. **TruEatz is not a medical device and does not diagnose, treat, cure, or prevent any medical condition. Always consult a qualified healthcare professional for medical advice, diagnosis, or treatment.**

We have completed Google Play's Health Apps Declaration where required and operate as a non-medical-device wellness / nutrition information app.

---

## 16. Changes to This Policy

We may update this Policy as the App evolves. When we make material changes, we will:
- Update the "Last Updated" and "Version" fields above
- Notify you in the App or by email at least 30 days before changes take effect
- Provide a plain-language summary of what changed
- Give you the chance to review and, if you disagree, delete your account before changes apply

**Material changes** include changes to data practices, data sharing partners, retention periods, your rights, or the legal basis for processing.

**Non-material changes** (typo fixes, formatting, contact information updates, clarifications without substantive impact) take effect immediately upon posting.

If you continue using TruEatz after changes take effect, you accept the updated Policy.

A historical archive of prior versions is available on request via app@trueatzapp.com.

---

## 17. Contact Us

Questions, concerns, or want to exercise your rights?

**Email:** app@trueatzapp.com

**Subject prefixes:**
- "Privacy Request" — general privacy question
- "California Privacy Request" — CCPA / CPRA rights
- "GDPR Request" — EEA or UK rights
- "COPPA Request" — children's privacy
- "Security" — vulnerability or breach report
- "Data Export" — request a portable copy of your data

We respond to all privacy requests within 30 days (45 days for CCPA / California requests where allowed by law).

---

*TruEatz — Real food. Real science. No tracking. No selling. No ads.*
