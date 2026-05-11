# Privacy Policy

**Effective date:** May 11, 2026
**Last updated:** May 11, 2026
**App:** ARIA: AI Personal Assistant
**Operator:** Boris Legkow (sole proprietor) — contact: blegkow@gmail.com

This Privacy Policy explains how ARIA ("ARIA", "we", "our", "the App") collects, uses, stores, and shares information when you use the iOS application "ARIA: AI Personal Assistant". By using ARIA you agree to the practices described here. If you do not agree, do not install or use the App.

We've tried to write this in plain English. Where law requires more formal language, we've included it.

---

## 1. What information we collect

### 1.1 Information you give us directly
- **Account profile** — your first name, email address (from Sign in with Apple or Google), and theme/currency preferences.
- **Tasks, calendar events, reminders, notes** — content you create inside ARIA.
- **Financial data you import manually** — bank statement PDFs you upload, receipt photos you scan, transactions you type in, budget categories, financial goals, and contributions.

### 1.2 Information collected through connected services (only if you opt in)
- **Plaid (bank linking)** — if you connect a bank through Plaid, Plaid collects your bank login credentials, account balances, transaction history, account/routing numbers, and account holder name. Plaid sends ARIA your transactions and balances; **Plaid does NOT share your login credentials with us**. See Plaid's End User Privacy Policy at https://plaid.com/legal/#end-user-privacy-policy.
- **Apple/Google Calendar** — if you grant calendar permission, ARIA reads event titles, times, and locations to display your schedule. We do not write to your calendar without your action.
- **Apple Reminders** — if you grant reminders permission, ARIA reads reminder text and due dates.
- **Photos / Camera** — only when you scan a receipt or import a PDF statement. The image/file is sent to Anthropic for parsing and is not retained by us beyond the import session.
- **Microphone** — only if you tap the voice input button. Audio is sent for transcription and not retained.
- **Notifications** — to deliver bill reminders and trial-end reminders. You can disable in iOS Settings at any time.

### 1.3 Information collected automatically
- **Crash and performance data** — collected by Sentry to help us diagnose bugs. This may include device model, OS version, app version, anonymized IP address, and a stack trace of the error. We do not associate this with your account profile unless required to investigate a specific reported issue.
- **Subscription status** — managed by RevenueCat. RevenueCat receives a pseudonymous user ID, your subscription tier, trial state, and renewal events. No payment card details are seen by ARIA or RevenueCat — payment is handled entirely by Apple (or Google) through your device's App Store account.

### 1.4 Information we do NOT collect
- Your bank login credentials (handled by Plaid)
- Your payment card details (handled by Apple/Google)
- Your precise location
- Your contacts (we do not request contacts permission)
- Your browsing history outside the App
- Advertising identifiers (IDFA) — ARIA does not run ads

---

## 2. How we use your information

We use the information described above only to:
- Provide the App's core features (track tasks, surface bills, analyze spending, generate AI summaries)
- Personalize your experience (greet you by name, adapt to your timezone/currency)
- Send local push notifications you've enabled (bill reminders, trial end)
- Improve the App by understanding which features users hit (basic usage metrics) and what causes crashes (Sentry)
- Process subscriptions via RevenueCat and Apple/Google's billing systems
- Comply with legal obligations (respond to lawful requests, prevent fraud)

We do NOT use your data to:
- Train any AI model (yours or anyone else's). Specifically: prompts sent to Anthropic's Claude API are processed under Anthropic's API terms and are not used for training (see https://www.anthropic.com/legal/aup and https://www.anthropic.com/legal/privacy).
- Sell to data brokers or marketers
- Profile you for advertising

---

## 3. Who we share your data with

We share data only with the third-party processors needed to run the App. Each is bound by their own privacy policy and (where applicable) a data processing agreement.

| Processor | What we share | Why | Their privacy policy |
|---|---|---|---|
| **Apple** | Sign in with Apple identifier, App Store transaction records | Authentication, subscription billing | https://www.apple.com/legal/privacy/ |
| **Google** | Sign in with Google identifier (if used) | Authentication | https://policies.google.com/privacy |
| **Plaid** | Bank credentials (entered directly by you in Plaid's UI, never seen by us) | Bank account linking | https://plaid.com/legal/ |
| **Anthropic (Claude API)** | Text prompts and uploaded PDFs/images you submit for AI processing | Generate AI summaries, parse statements, scan receipts | https://www.anthropic.com/legal/privacy |
| **RevenueCat** | Pseudonymous user ID, subscription status | Subscription management | https://www.revenuecat.com/privacy |
| **Sentry** | Crash/performance telemetry, anonymized IP | Diagnose bugs | https://sentry.io/privacy/ |
| **Cloudflare** | Backend traffic metadata (request URLs, timing) | Host our API | https://www.cloudflare.com/privacypolicy/ |

We do **not** sell your personal information. We do not share your data with advertisers.

If we are legally compelled (e.g., a valid subpoena or court order), we will comply only to the minimum extent required and will notify you unless prohibited by law.

---

## 4. Where your data lives

- **On your device** — most of ARIA's data lives locally on your iPhone in encrypted AsyncStorage. This includes tasks, transactions you've manually entered, budgets, and goals.
- **On our backend** — our backend runs on Cloudflare Workers (global edge). The Worker stores only session tokens and pseudonymous user identifiers, not your actual financial data.
- **With Anthropic** — prompts/files you send for AI processing are transmitted to Anthropic in the United States and processed under their API terms. They are not retained for training.
- **With Plaid** — transaction history retrieved from your bank is held by Plaid in the US.
- **With RevenueCat** — subscription state is held by RevenueCat in the US.
- **With Sentry** — crash data is held by Sentry in the US.

---

## 5. How long we keep your data

- **Account profile** — for as long as your account is active. If you delete your account, we delete it within 30 days.
- **On-device data** — kept until you uninstall ARIA or use "Reset App" in Settings.
- **Anthropic prompts** — Anthropic retains prompts according to their API policy (typically up to 30 days for abuse monitoring) and does not train models on them.
- **Plaid data** — Plaid's retention is governed by their privacy policy.
- **Sentry crash data** — retained 30 days for error triage.

---

## 6. Your rights

Regardless of where you live, you can:
- **Access** your data — most of it is visible in the App; for backend data, email blegkow@gmail.com.
- **Correct** inaccurate information — edit profile, transactions, and tasks directly in the App.
- **Delete** your account — Settings → Delete Account. This wipes local data and clears your server-side session within 30 days.
- **Export** your data — email blegkow@gmail.com and we'll send a JSON dump within 30 days.
- **Disconnect** bank links — Finance tab → Connected Banks → Disconnect.

### 6.1 European Economic Area, UK, and Switzerland (GDPR)
You have the additional rights to: object to processing, restrict processing, lodge a complaint with your local data protection authority, and request portability of your data in a machine-readable format. Our lawful basis for processing is your consent (which you can withdraw any time by uninstalling) and the performance of our contract with you (delivering the App).

### 6.2 California (CCPA / CPRA)
California residents have the right to know what categories of personal information we collect, to delete it, to correct it, and to opt out of any "sale" or "sharing" (we don't sell or share, but you have the right to be told). We do not discriminate against you for exercising these rights.

### 6.3 Other US states (Colorado, Connecticut, Texas, Virginia, etc.)
We honor the rights granted by applicable state privacy laws. Contact us at blegkow@gmail.com.

---

## 7. Children

ARIA is not directed at children under 13 (under 16 in the EU) and we do not knowingly collect data from them. If you are a parent and believe your child has provided us data, contact us and we will delete it.

---

## 8. Security

- All network traffic to and from the App uses HTTPS / TLS 1.2+.
- On-device data sits in iOS's encrypted file system, protected by your device passcode/biometrics.
- Backend secrets (API keys) are stored in Cloudflare Workers' secret store, never in client code.
- We do not store passwords (auth is delegated to Apple / Google).

No system is 100% secure. If a breach affecting your data occurs, we will notify affected users and applicable regulators as required by law.

---

## 9. International transfers

If you use ARIA outside the United States, your data may be transferred to and processed in the US (where our processors are based). We rely on Standard Contractual Clauses (or equivalent legal mechanisms) for transfers from the EEA/UK/Switzerland to the US.

---

## 10. Changes to this policy

We may update this policy. If changes are material, we will surface a notice in the App before they take effect. The "Effective date" at the top of this document is the date of the most recent material update.

---

## 11. Contact

Questions, requests, or complaints:

**Boris Legkow**
Email: blegkow@gmail.com

If you contact us about a privacy request, we will respond within 30 days.
