# ClickDebt

**Clear your landing page’s ClickDebt in 30 seconds.**

ClickDebt is a cosy, quirky indie web app & PWA that audits any public landing page URL using **Google Gemini 2.5 Flash**, delivers an instant **Free ClickDebt Score (0–100) + Top 3 Conversion Leaks**, and lets founders pay **$9 one-time via Stripe Checkout** to unlock a complete **Debt-Free Rewrite Pack**:

- Side-by-side **Before → After Hero Rewrite** (Headline, Subheadline, Primary & Secondary CTAs, Trust Line)
- **5 Objection-Busting FAQs** tailored to the audited site
- **3 Pricing & Offer Tune-Ups** with impact stamps
- **Interactive 6-step Launch Checklist** (persisted in `localStorage`)
- **One-click Markdown Export** & print-styled **PDF Studio Keepsake**

## Quick Start (Local)

1. Install dependencies:
   ```bash
   npm install
   ```
2. Copy `.env.example` to `.env.local` and add your keys:
   ```bash
   cp .env.example .env.local
   ```
   - `GEMINI_API_KEY` — get one free/pay-as-you-go at [Google AI Studio](https://aistudio.google.com/apikey)
   - `STRIPE_SECRET_KEY` — grab your `sk_test_...` or `sk_live_...` key from the Stripe Dashboard (leave empty to test unlock in Demo Mode)
3. Start the dev server:
   ```bash
   npm run dev
   ```

## Ship to Market Tonight (Vercel)

1. Import this GitHub repository in [Vercel](https://vercel.com/new).
2. Add Environment Variables:
   - `GEMINI_API_KEY`
   - `STRIPE_SECRET_KEY` (`sk_live_...` when ready to collect real $9 payments)
   - `UNLOCK_SIGNING_SECRET` (any random 32+ character string)
   - `NEXT_PUBLIC_APP_URL` (your live domain, e.g. `https://clickdebt.app`)
3. Click **Deploy** — zero database setup required! Paid reports are verified directly against Stripe Checkout sessions and include automatic cold-start recovery.
