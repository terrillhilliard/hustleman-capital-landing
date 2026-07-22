# Hustleman Capital — Landing Page

Static marketing site (plain HTML/CSS/JS, no build step). Deploy target: Vercel (static).

## Structure
- `index.html` — main landing page
- `pricing.html` — pricing page
- `images/` — gallery photos
- `lib/` — self-hosted `ogl` (circular gallery) + `gsap` (card effects)
- `CLIENT-CHECKLIST.md` — content the client must supply/verify

## ⚠️ Before pointing the production domain here
This is a **review/staging build**. Do NOT treat it as final until:

1. **Verify every claim** marked `*` on the page — member count (245K), AI win rate (98%),
   and the "$100M+ / $40M / $30M …" track-record figures. Document or remove each.
2. **Rick Ross partnership** — requires written authorization before featuring the name/photo.
3. **Wire the backends** (currently save to `localStorage` only — search the code for `TODO`):
   - Email signup CTA (hero + final)
   - Guided chat assistant lead capture
   - Inquiry form
   - Promo 20% coupon code at checkout
4. **Swap the live news feed** — currently the unofficial ESPN public API; use a licensed feed for production.
5. Legal review of gambling / income / credit / investment disclaimers.

## Local preview
Serve over HTTP (ES modules + WebGL need a server, not `file://`):
```
python -m http.server 5566
```
