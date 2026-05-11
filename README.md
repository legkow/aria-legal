# ARIA Legal Documents

This folder contains the **source of truth** for ARIA's Privacy Policy and Terms of Service. These documents are required by the App Store and Google Play for submission.

## Files

- `privacy-policy.md` — Privacy Policy v1
- `terms-of-service.md` — Terms of Service v1

## How to host them publicly

You need both documents at **stable, publicly accessible HTTPS URLs**. The App Store rejects submissions with broken or missing links.

### Fastest option: GitHub Pages (free, ~5 min)

1. Create a new public GitHub repo: `aria-legal`
2. Drop both `.md` files in the repo root
3. In repo Settings → Pages → enable Pages on the `main` branch
4. GitHub renders the markdown automatically. URLs will be:
   - `https://blegkow.github.io/aria-legal/privacy-policy`
   - `https://blegkow.github.io/aria-legal/terms-of-service`

### Alternative: Vercel (free, ~5 min)

1. `npm i -g vercel`
2. Create `index.html` files that embed the rendered markdown
3. `vercel deploy --prod`
4. Set a custom domain like `legal.aria.app` if you have one

### Alternative: your Squarespace site

1. Create two new pages titled "Privacy Policy" and "Terms of Service"
2. Paste each rendered markdown body into the page editor
3. URLs become e.g. `https://yoursite.com/privacy` and `https://yoursite.com/terms`

## Where to use the URLs

Once hosted, paste the URLs into:

1. **App Store Connect** → App Information → Privacy Policy URL (required)
2. **App Store Connect** → App Information → Support URL (link the privacy policy or a contact page)
3. **App Store Connect** → App Privacy Nutrition Labels — fill these out to match what the policy says you collect
4. **ARIA app** → Settings tab → add "Privacy Policy" and "Terms of Service" rows that open these URLs in a browser
5. **Onboarding paywall** → small text below subscribe button: "By subscribing you agree to the Terms of Service and Privacy Policy"

## Important caveats

- **These are starter documents tailored to ARIA's actual data flows.** They are not legal advice. Before public launch with real users, consider paying a lawyer for ~1 hour of review (~$300) or upgrading to Termly ($10/mo) for continuously-maintained compliance.
- **Privacy laws change frequently.** GDPR, CCPA, CPRA, Texas TDPSA, Florida FIPA — at minimum, review and re-issue these documents annually.
- **Apple cross-references the policy text against the Privacy Nutrition Labels in App Store Connect.** A mismatch can trigger rejection. After hosting the policy, walk through the Nutrition Labels and check that every data category disclosed matches.
- **If you incorporate or move to an LLC**, update the operator name in both documents.

## Updating

When you need to update either document:

1. Edit the `.md` file here
2. Bump the "Effective date" and "Last updated" lines at the top
3. Re-publish to your host
4. If changes are material, notify users in-app (Privacy Policy section 10 / ToS section 14 require this)
