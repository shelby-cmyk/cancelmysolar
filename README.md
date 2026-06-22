# cancelmysolar.co

Single-page CPA lead-gen lander for solar contract cancellation. Static HTML, no build step.

## Files
- `index.html` — the lander (phone + form co-equal CTAs)
- `privacy.html` / `terms.html` — required for consent links + ad-platform approval
- `CNAME` — `cancelmysolar.co` (for GitHub Pages / Cloudflare Pages)

## Before going live — wiring checklist
Search `index.html` for these markers:

- **`PHONE_NUMBER`** — replace `(800) 555-0123` and the `tel:+18005550123` links (header, hero, CTA band, footer, mobile bar, form success) with the real click-to-call number. This is half your CPA revenue — get the tracking number right.
- **`LEAD_ENDPOINT`** (in the `<script>`) — set to your buyer/CRM/webhook URL so form fills POST as JSON. The payload includes all fields + captured consent language + timestamp + page URL. Left empty = form validates and shows success but only logs to console.
- **Privacy/Terms TODOs** — add registered business legal name + mailing address (ad platforms reject solar lead-gen without a real entity).
- **Tracking pixels** — add Google Ads / Meta pixel + conversion events on form submit and call click before running traffic.
- **Stats sourcing** — the 5M / 746% / $187 stats mirror the ExitSolar reference; confirm/replace with figures you can cite before scaling spend.

## Deploy
GitHub Pages or Cloudflare Pages — point cancelmysolar.co at it. CNAME already set.
