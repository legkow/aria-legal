# ARIA — App Store Listing Copy v1.1

**Updated 2026-05-11 based on Manus ASO audit.** Pivots from a generic "AI Personal Assistant" positioning to high-intent finance + planner terms. Title/subtitle/keywords are now optimized so Apple's algorithm reads them without double-counting.

Paste each section into App Store Connect → Distribution → App Information.

---

## App Name (30 chars max)

```
ARIA: AI Budget & Life Planner
```
(30 chars — exactly fits)

**Why:** "AI Personal Assistant" competes head-on with ChatGPT and Google Assistant searches. "AI Budget & Life Planner" captures higher-intent finance + planning searches with much less saturation.

---

## Subtitle (30 chars max)

```
Money manager, tasks & focus
```
(28 chars — fits)

**Why:** Title covers the "what it is", subtitle covers the "what it does". Three pain-point keywords (money manager, tasks, focus) all under-saturated.

---

## Promotional Text (170 chars max — editable without re-review)

```
Stop juggling 5 apps. ARIA brings your bills, tasks, calendar, and bank into one calm AI assistant — designed for messy brains, polished for everyone.
```
(150 chars)

**Why this wording:** dropped "AI co-pilot" (Microsoft trademark adjacency) → "AI assistant" (algorithm-friendly). Dropped "ADHD" up top → "messy brains" (universal). ADHD mention moves deeper into the description where engaged readers find it.

---

## Description (4000 chars max)

```
ARIA is your personal AI assistant for the parts of life that fight for your attention — money, tasks, time, and the one thing you should focus on today.

Most apps dump a wall of data on you and call it a dashboard. ARIA does the opposite. It reads what's on your plate, pre-decides what's actually important, and tells you the one next move. That's it.

WHAT ARIA DOES

• Daily Brief — every morning, ARIA reads your bills, tasks, calendar, and recent spending, then writes a single sentence telling you what to focus on today.

• Expense Tracker & Smart Money — connect your bank through Plaid (256-bit encrypted, read-only) or snap a photo of a receipt. ARIA acts as your personal bill organizer, categorizing everything, flagging duplicates, tracking subscriptions, and alerting you when a bill is about to hit.

• Safety Net — set a savings goal. ARIA shows you exactly how long it'll take to reach it at your current pace, and warns you when you're slipping.

• Tasks that respect your energy — drop tasks in plain English ("call dentist friday"), and ARIA schedules and reminds you. Long-press to change tags, swipe to complete.

• Calendar that thinks ahead — pulls from your existing iOS calendar and surfaces what's actually time-sensitive.

• AI Chat — ask ARIA anything about your money, time, or plans. Powered by Claude, with full context of your data (stored on-device).

PRIVACY FIRST

Your data lives on your iPhone. We never sell it. We never train AI on it. We use end-to-end TLS for the small bits that need a server. Sign in with Apple — no password needed, no email tracking.

For full details: https://legkow.github.io/aria-legal/privacy-policy

WHY THIS, WHY NOW

If you've ever:
- Opened 5 different apps to figure out if you can afford something
- Missed a bill because it was buried in email
- Felt overwhelmed by your task list at the start of every day
- Wished one app could just tell you "you're fine" or "act now"

— ARIA is for you.

DESIGNED FOR MESSY BRAINS

ARIA was built with neurodivergent minds in mind — especially ADHD. Pre-decided actions instead of infinite menus. One next step instead of a wall of options. Calm typography. No notification spam. If your attention is your most expensive currency, ARIA is built to spend less of it.

If that sounds like you — even some days — you'll feel the difference within an hour.

FOUNDERS PRICING (first 250 members)

$9.99/month or $79.99/year, locked at that rate for life.

After the founders cap is reached: $11.99/month or $99.99/year.

3-day free trial. Cancel anytime in iOS Settings.

WHAT YOU GET WITH PREMIUM

• Unlimited AI chat with full context
• Bank account linking via Plaid
• Bill auto-detection from imported statements
• Receipt scanning
• Daily Brief summaries
• Priority support

WHAT YOU CAN DO FOR FREE

• Manual transaction entry
• Tasks, calendar, and reminders
• Spending overview
• Basic ARIA insights
• Up to 5 AI chats per day

ARIA respects your attention. No notifications you didn't ask for. No dark patterns. No ads. Ever.

—

Terms of Service: https://legkow.github.io/aria-legal/terms-of-service
Privacy Policy: https://legkow.github.io/aria-legal/privacy-policy
Support: blegkow@gmail.com
```
(~2,650 chars)

**Two key changes from v1:**
1. The "Smart Money" bullet was rewritten to include exact-match phrases `Expense Tracker` and `bill organizer` — this is what AI crawlers (ChatGPT, Apple Intelligence) read when categorizing what ARIA is.
2. Removed the "former finance professional" line — keep it neutral until we know what's defensible.

---

## Keywords (100 chars max, comma-separated, NO spaces)

```
ADHD,finance,calendar,bills,assistant,reminder,expense,tracker,neurodivergent,routine,organizer
```
(95 chars)

**ASO rationale:**
- Dropped: `AI`, `planner`, `budget`, `life`, `focus`, `tasks` (already in title or subtitle — Apple double-counts these for free, no need to repeat)
- Dropped: `bank`, `money` (too generic for a new app to rank)
- Added: `expense`, `tracker`, `neurodivergent`, `routine`, `organizer` (higher-intent niche terms)

**Post-launch:** watch which terms drive installs in App Store Connect → Analytics; rotate the bottom 3 monthly.

---

## Support URL (required)

```
https://legkow.github.io/aria-legal/
```

---

## Marketing URL (optional)

Leave blank for v1. Add a Squarespace/Carrd landing page later.

---

## Copyright

```
© 2026 Boris Legkow
```

---

## Age Rating

When prompted, answer **No** to all categories EXCEPT:
- **Unrestricted Web Access** → "No" (Plaid bank login is domain-restricted)
- **Frequent/Intense Medical/Treatment Information** → No

Target rating: **4+**.

---

## Category

- **Primary:** Finance
- **Secondary:** Productivity

---

## Subscription Display Names

For each subscription product in App Store Connect → Subscriptions:

**aria_founders_monthly:**
- Display Name: `ARIA Premium — Founders Monthly`
- Description: `All AI features, bank sync, and Daily Brief — founders rate locked for life`

**aria_founders_annual:**
- Display Name: `ARIA Premium — Founders Annual`
- Description: `Save 33% with annual — founders rate locked for life`

**aria_monthly:**
- Display Name: `ARIA Premium Monthly`
- Description: `All AI features, bank sync, and Daily Brief`

**aria_annual:**
- Display Name: `ARIA Premium Annual`
- Description: `Save 33% with annual billing`

---

## Notes for v1 review

- Founders pricing is auto-selected for the first 1,000 — only the founders SKUs go live initially
- Reviewers may ask for a demo account: tell them `blegkow@gmail.com` with **Settings → Test Mode** toggled ON unlocks gated features
- If Apple asks about AI: "ARIA uses Anthropic's Claude API for natural-language responses via a server-side proxy. The API key is never in the client."

---

## Post-launch ASO playbook (Manus audit recommendations)

1. **Apple Search Ads** — run small discovery campaigns targeting "Copilot Money" and "Tiimo" audiences (high-overlap users)
2. **Review mining** — after 50+ reviews, harvest the exact phrases users describe ARIA with ("best ADHD budget", "saved my brain", etc.) and feed those into the subtitle or keyword field in month 3
3. **In-App Events** — Apple now indexes these on the web. Schedule one for a real moment (e.g. "New Year Financial Reset", "Tax-Time Sweep") to boost discoverability
4. **Localized listings** — once core is stable, add localized title + keywords for fr-CA, es-MX, en-GB (different keyword saturation in each)

---

## Competitor positioning (from Manus audit)

| App | Title | Subtitle | Lesson |
|---|---|---|---|
| Copilot | Copilot: Track & Budget Money | Spending, investing, net worth | Brand + high-volume keywords |
| Tiimo | Tiimo: To-Do List & AI Planner | Daily Routine & Habit Planning | Visual planner for ADHD |
| Cleo | Cleo AI: Cash Advance & Budget | Build Credit, Save Money | Sassy AI for Gen Z |
| neurolist | neurolist: AI Planner for ADHD | neurodivergent task splitter | Niche AI for ADHD task breakdown |

ARIA sits between Copilot (full money) and Tiimo (full ADHD productivity) — uniquely positioned to capture both intents with a single listing.
