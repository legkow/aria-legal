# ARIA — Privacy Policy

**Last updated: 29 June 2026**
**Effective date: 29 June 2026**

This Privacy Policy explains how ARIA ("ARIA", "the app", "we", "us", "our")
handles your information. ARIA is a personal-finance, calendar, and task
assistant for iPhone. It is built around a simple promise: **your data lives on
your device, and we never sell it.**

ARIA is provided by **Boris Alexander Legkow Orias**, an individual developer
operating as a sole trader in **Quebec, Canada** ("the developer"). The developer
is the enterprise responsible for your personal information under **Quebec's
Law 25** (the Act respecting the protection of personal information in the private
sector), the federal **PIPEDA**, and — for users in those regions — the **EU/UK
GDPR** (as data controller) and the **California CCPA/CPRA**.

- **Person in charge of the protection of personal information (Privacy Officer):**
  Boris Alexander Legkow Orias
- **Contact:** legkow@me.com
- **Postal address:** 1 rue Boucher, Port-Cartier, QC G5B 2T9, Canada
- **Website:** https://legkow.github.io/aria-legal

Quebec residents are covered by **Law 25**; other Canadian users and any personal
information that crosses provincial or national borders are covered by **PIPEDA**.
Where more than one law could apply, we apply the **higher standard**.

> **Plain-language summary.** Almost everything you put into ARIA stays on your
> iPhone. If you turn on sync, your data is encrypted on your device with a key
> that never leaves it, so even we cannot read it. Some features are optional and
> only run when you switch them on: connecting a bank (Plaid) or importing your
> calendar (Google/Apple). AI
> features run on your device using Apple's models. We do not track you across
> apps or websites, we run no advertising SDKs, and we do not sell your data.
> This summary is for convenience only; the full text below governs.

---

## 1. Who this policy covers

This policy applies to everyone who uses the ARIA iOS app. It covers data you
enter, data ARIA reads from services you choose to connect, and the limited data
needed to run your account and subscription.

ARIA is intended for a **general audience of adults**. It is **not directed to
children**, and we do not knowingly collect their data: not from a minor under
**14** in Quebec (the age Law 25 keys parental consent to), under **16** in the
EU/UK, or under **13** in the United States. See Section 11.

---

## 2. The data ARIA handles, and where it lives

ARIA is **local-first**. Unless a row below says data is "transmitted," it is
stored only on your device (in Apple's SwiftData store and the iOS Keychain) and
is never sent to us or anyone else.

| Data | Examples | How ARIA gets it | Where it goes |
|---|---|---|---|
| **Financial records** | Account names & balances, transactions (merchant, amount, date, category), bills, budgets, goals, safety-net amounts, subscriptions | You enter it; you import a CSV; or you link a bank via Plaid | On device. If sync is on, included in the **end-to-end-encrypted** backup. |
| **Bank data via Plaid** | Account balances, transaction history, account mask (last 4 digits) | Only if you connect a bank in Plaid Link | Fetched server-side by our backend and delivered to your device. See Section 5. **Read-only — ARIA never moves money.** |
| **Calendar events** | Event titles, dates, times | Apple Calendar (EventKit) and/or Google Calendar, read-only, only if you connect them; or you create events in ARIA | On device. If sync is on, included in the encrypted backup. |
| **Tasks & projects** | Task titles, due dates, tags, projects, steps | You enter them, or add them by voice via Siri | On device. If sync is on, included in the encrypted backup. |
| **Your name** | First name | You optionally provide it at sign-in | On device; tied to your account if you use cloud sync. |
| **Account identifier** | Apple user identifier (from Sign in with Apple) | Sign in with Apple | Sent to our backend to create and authenticate your account. |
| **Receipt photos** | A photo of a receipt | Only if you scan a receipt | Processed **on device** to read merchant/amount/date, then **discarded**. The image is never stored or transmitted. |
| **Voice input** | What you say while holding the talk control | Microphone + on-device speech recognition | Transcribed **on your device** (`requiresOnDeviceRecognition`), used to answer, then discarded. Not stored, not transmitted. |
| **Face ID / biometrics** | Biometric match result | Optional app lock | Handled entirely by iOS (LocalAuthentication). ARIA never sees or stores biometric data. |
| **Diagnostics (optional)** | Coarse, non-identifying usage events (e.g. "feature opened") | Only if you turn on "Usage analytics" (off by default) | See Section 6. Contains no names, emails, or amounts. |
| **Subscription/purchase state** | Whether you have ARIA+ | App Store purchase via RevenueCat | See Section 5. |
| **Device settings** | Appearance, currency, language, ARIA's personality, notification preferences | You set them | On device (`UserDefaults` / `@AppStorage`). |

We do **not** collect: your bank login credentials (those go directly to Plaid,
never to ARIA), your precise location, your contacts, advertising identifiers,
or your full email content.

---

## 3. Why we process your data, and our legal bases (GDPR)

Where the GDPR/UK GDPR applies, we rely on the following legal bases (Art. 6):

| Purpose | Legal basis |
|---|---|
| Run the app's core features on your device (track money, bills, tasks, calendar) | **Performance of a contract** (Art. 6(1)(b)) — you asked us to provide ARIA |
| Authenticate your account and sync your encrypted backup | **Performance of a contract** (Art. 6(1)(b)) |
| Connect a bank (Plaid) or import a calendar (Google/Apple) | **Consent** (Art. 6(1)(a)) — these are off until you switch them on, and you can withdraw at any time |
| Process biometric app-lock | **Consent** — and handled by iOS, never by us |
| Optional diagnostics | **Consent** (off by default) |
| Manage your ARIA+ subscription | **Performance of a contract** (Art. 6(1)(b)) |
| Keep the service secure, prevent abuse, and meet legal obligations | **Legitimate interests** (Art. 6(1)(f)) and **legal obligation** (Art. 6(1)(c)) |

You can withdraw consent at any time by disconnecting the relevant integration
in Settings or turning the feature off. Withdrawing consent does not affect
processing that already happened.

**Consent, and express consent for sensitive data.** We ask for your consent
through clear, specific, separate choices — each optional integration (Plaid,
Google Calendar) and cloud sync are off until you turn them on. Because
your **financial information is sensitive**, we ask for your **express** consent
before you connect a bank or we process your financial data, and we use it only
for the purposes you enabled.

---

## 4. On-device intelligence and AI

ARIA's "intelligence" — the Life Score, proactive nudges, receipt reading,
subscription detection, anomaly flags, and the voice assistant — runs **on your
device** using Apple's on-device **Foundation Models**, with deterministic
on-device logic for scoring and pattern detection.

- Where a request needs more capability than the on-device model provides, iOS
  may use **Apple Private Cloud Compute** — Apple's privacy-preserving server
  environment. You can pin ARIA to **strictly on-device** processing in Settings
  ("On-device only"), which keeps these features fully offline.
- **We do not send your data to any third-party AI provider** (no OpenAI, no
  Anthropic, no Google AI). There is no per-token cloud AI in ARIA.
- AI output is informational and may be wrong. ARIA surfaces patterns in your own
  data; it does **not** provide financial, investment, tax, or legal advice. See
  the Terms of Use.
- **Automated processing and profiling.** ARIA builds insights from a profile of
  your own data (the Life Score, "safe-to-spend," anomaly flags, nudges). These
  are **informational** and are **not** decisions made solely by a machine with
  legal or similarly significant effects — you decide what to do. If we ever
  introduced such an automated decision, we would tell you, explain the main
  factors used, let you have the underlying data corrected, and let you ask a
  person to review it.

---

## 5. Third-party services we work with

ARIA uses a small number of providers. We share **only what each feature needs**,
and only when you use that feature. Each provider is an independent controller or
processor under its own privacy policy.

### Plaid — bank connection (optional)
If you connect a bank, you do so through **Plaid Link**. You enter your bank
credentials **directly with Plaid** — ARIA never sees or stores them. Plaid
returns account and transaction data, which our backend retrieves on your behalf
and delivers to your device. The Plaid access token is held **server-side only**;
your device holds only an opaque item identifier. The connection is **read-only**;
ARIA cannot and does not move money, make payments, or initiate transfers.
Your use of Plaid is also governed by Plaid's **End User Privacy Policy**:
https://plaid.com/legal/#end-user-privacy-policy. You can disconnect a bank at any
time in Settings, which unlinks the item.

### Google — Calendar (optional)
If you connect Google Calendar, ARIA requests **read-only** access
(`calendar.readonly`) via Google OAuth. OAuth tokens are stored in your device
Keychain.

> **Limited Use disclosure.** ARIA's use and transfer of information received from
> Google APIs adheres to the
> [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy),
> including its **Limited Use** requirements. Specifically: we access Google
> Calendar data only to provide and improve the in-app features you request
> (showing your events); we process this data **on your device**; we do **not**
> transfer it to others except as needed to provide these features, for security,
> or to comply with law; we do **not** use it for advertising; and we do **not**
> allow humans to read it except with your consent, for security, or as required
> by law.

### Apple — accounts, calendar, purchases, intelligence
ARIA uses Apple frameworks: **Sign in with Apple** (account creation), **EventKit**
(Apple Calendar), **StoreKit** (purchases), **Speech** (on-device transcription),
**LocalAuthentication** (Face ID), **ActivityKit** (Live Activities), and
**Foundation Models / Private Cloud Compute** (intelligence). Apple's handling of
this data is governed by Apple's Privacy Policy (https://www.apple.com/legal/privacy/).

### RevenueCat — subscription management
ARIA+ subscriptions are processed through Apple's App Store and managed using
**RevenueCat**, which validates your App Store receipt and tells the app whether
your subscription is active. RevenueCat receives a pseudonymous app user ID and
purchase/receipt data; it does not receive your financial records, calendar, or
email. See RevenueCat's privacy policy: https://www.revenuecat.com/privacy.

### Cloudflare — our backend and encrypted sync
Our account, sync, and Plaid backend runs on **Cloudflare Workers** (in the
United States). It stores your **end-to-end-encrypted** sync backup (which we
cannot decrypt), your account record, and — server-side only — your Plaid access
token. Cloudflare acts as our hosting processor.

We maintain a current list of sub-processors available on request at
legkow@me.com.

---

## 6. Analytics and tracking

- ARIA ships **no advertising SDKs** and performs **no cross-app or cross-site
  tracking**. We do not use the Advertising Identifier (IDFA) and do not present
  an App Tracking Transparency prompt because we do not track you. Our Apple
  Privacy Manifest declares **"Data not used to track you."**
- **Usage analytics are opt-in and off by default.** If you turn them on in
  Settings, ARIA records only coarse, **non-identifying** events (such as which
  feature was opened) — never your name, email, or any money amount. Turning the
  setting off erases what was stored. If we transmit these diagnostics, our
  processor is **PostHog**; events remain free of personal identifiers.

---

## 7. How we share data

We **do not sell** your personal information, and we **do not "share" it for
cross-context behavioral advertising** as those terms are defined under the
California Consumer Privacy Act (CCPA/CPRA). We have not sold or shared personal
information in the preceding 12 months.

We disclose data only:
- to the providers in Section 5, strictly to run the features you use;
- if required by law, legal process, or a valid government request;
- to protect the rights, safety, or security of users or the public; or
- in connection with a business transfer (e.g. if the app is acquired), in which
  case we will notify you and this policy will continue to apply to your data.

---

## 8. Data retention

- **On-device data** stays until you delete it, delete the app, or delete your
  account.
- **Encrypted sync backup** is retained while your account is active and deleted
  when you delete your account (see Section 9).
- **Receipt images** are never stored — they are processed once and discarded.
- **Voice input** is ephemeral and discarded after it is used to answer you.
- **Optional diagnostics** are capped to a small local buffer and cleared when you
  turn analytics off.
- **Account and Plaid records** on our backend are deleted when you delete your
  account, subject to any short retention required for security or legal reasons.

---

## 9. Your rights and choices

**In-app controls (available to everyone):**
- **Export my data** — download a complete JSON copy of your records (Settings → Data).
- **Delete account** — erases your account on our backend and every record on your
  device, and destroys your sync encryption key. This cannot be undone.
- **Disconnect integrations** — unlink Plaid or Google Calendar at any time.
- **Turn off sync / use offline** — keep all data on-device only.
- **Turn off diagnostics** — clears stored events.

**EU/UK (GDPR) rights.** You may request access, rectification, erasure,
restriction, portability, and objection, and you may withdraw consent at any time.
Many of these are available directly in-app (export/delete). For anything else,
email legkow@me.com. We respond within **30 days** (extendable by 60 days for
complex requests). You also have the right to lodge a complaint with your
supervisory authority. *(Note: a non-EU controller offering services to EU users
may be required to appoint an EU representative under GDPR Art. 27 — see "Action
needed" handoff.)*

**California (CCPA/CPRA) rights.** You may request to know, delete, and correct
your personal information, and to limit the use of sensitive personal information.
We do not sell or share your personal information and do not discriminate against
you for exercising your rights. We acknowledge requests within **10 business days**
and respond within **45 days** (extendable by 45 days). Submit requests at
legkow@me.com.

**Canada — Quebec (Law 25) & PIPEDA rights.** You may:
- **access** the personal information we hold about you and **correct** it;
- receive the information you gave us in a **structured, commonly used format**
  (we provide **JSON**) — **data portability** — or have it sent to another
  organization you authorize (this covers information you provided, not values
  ARIA infers, such as the Life Score);
- **withdraw your consent** at any time, and ask us to stop disseminating or to
  de-index your information where the law allows;
- be informed about any automated processing, as described in Section 4.

We respond within **30 days**. If we refuse a request, we explain why and tell you
how to seek a review. You can also complain to a regulator: in **Quebec**, the
**Commission d'accès à l'information (CAI)** — cai.gouv.qc.ca; elsewhere in
**Canada**, the **Office of the Privacy Commissioner of Canada (OPC)** —
priv.gc.ca, 1-800-282-1376. We make this policy publicly available and will
provide a copy on request.

We verify requests using reasonable measures proportionate to the data involved
(for example, control of the account email).

---

## 10. Security

- **End-to-end encryption.** Your sync backup is encrypted on your device with
  **AES-256-GCM** using a 256-bit key derived and held in your device Keychain.
  The key **never leaves your device** and is never sent to our servers, so we
  cannot read your synced data.
- **In transit**, all network traffic uses HTTPS/TLS.
- **At rest on device**, credentials and keys are stored in the iOS Keychain
  (`ThisDeviceOnly`); bank credentials are never handled by ARIA.
- No method of storage or transmission is 100% secure. If a **confidentiality
  incident** (data breach) occurs, we assess the risk and respond as the law
  requires:
  - **Quebec (Law 25):** where the incident presents a **risk of serious injury**,
    we notify the **Commission d'accès à l'information** and affected individuals
    with diligence, and we keep a register of incidents.
  - **Canada (PIPEDA):** where a breach creates a **real risk of significant
    harm**, we report it to the **Office of the Privacy Commissioner of Canada**
    and notify you as soon as feasible.
  - **EU/UK (GDPR):** we notify the relevant supervisory authority within **72
    hours** where required, and affected users without undue delay where the risk
    is high.

---

## 11. Children

ARIA is not directed to children. We do not knowingly collect personal
information from a minor under **14** in Quebec (where Law 25 keys consent to a
parent or tutor), under **16** in the EU/UK, or under **13** in the United States
(COPPA). If you believe a child has provided us data, contact legkow@me.com
and we will delete it.

---

## 12. Communication outside Quebec / Canada, and international transfers

Our backend and service providers (Cloudflare, RevenueCat, Plaid, Google) are
located in or process data in the **United States** — so some of your information
(your account record; if you link a bank, a server-side access token; and your
end-to-end-encrypted sync backup) is **communicated outside Quebec and Canada**.

- For **Quebec** residents, before relying on a provider outside Quebec we conduct
  the privacy impact assessment Law 25 requires and put a written agreement in
  place; our case rests on **end-to-end encryption** (the US host cannot read your
  synced content) and on data minimization.
- For other **Canadian** users, we remain accountable under PIPEDA and require our
  providers to protect your data by contract to a comparable standard.
- For **EU/UK** users, transfers rely on appropriate safeguards including the **EU
  Standard Contractual Clauses** and the **UK International Data Transfer Addendum**.

Your **synced content is end-to-end encrypted and unreadable in transit and at
rest** by us and our hosting provider.

---

## 13. Changes to this policy

We may update this policy as the app evolves or the law changes. We will post the
updated version with a new "Last updated" date and, for material changes, provide
in-app notice. Continued use after an update means you accept the revised policy.

---

## 14. Contact

Questions, requests, or complaints:
**legkow@me.com**
Boris Alexander Legkow Orias · 1 rue Boucher, Port-Cartier, QC G5B 2T9, Canada

---

*ARIA is an informational tool. It is not a bank, money transmitter, or financial
adviser, and it does not move money. See the [Terms of Use](./terms-of-service) for details.*
