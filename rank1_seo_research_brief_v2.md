# SEO & AEO Research Brief v2 — Rank 1 Accounting
## UPDATED June 9, 2026 — Corrected for May/June 2026 Google Changes
## For Claude Code: Read every line before writing any code.

---

## ⚠️ CRITICAL UPDATE — MAY 2026 SCHEMA CHANGE

**FAQPage schema NO LONGER generates rich results in Google Search.**
As of May 7, 2026, Google officially removed FAQ rich results entirely.
FAQPage schema is NOT dead — it still helps ChatGPT, Perplexity, and Google AI Mode parse and cite your content. But do NOT promise it will show FAQ dropdowns in Google Search results. It won't.

**What this means for the build:**
- Keep FAQPage schema for AI citation value (ChatGPT, Perplexity, AI Overviews)
- Keep FAQ sections visible on every page for AEO and user experience
- Do NOT rely on FAQ schema for Google SERP visual features

---

## 1. CORE WEB VITALS — EXACT TARGETS (Google Official, confirmed 2026)

All three must pass at the 75th percentile of real visitors:

- **LCP:** Under 2.5 seconds
- **INP:** Under 200 milliseconds  
- **CLS:** Under 0.1

### Technical implementation rules:
- Inline all critical CSS in `<head>` — no render-blocking stylesheets
- System fonts only: `font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif`
- Hero image: WebP format + `fetchpriority="high"` + preload in `<head>` — NEVER lazy load hero
- All below-fold images: `loading="lazy"` + explicit `width` and `height` attributes
- No jQuery — vanilla JS only
- Defer all non-critical JS with `defer` attribute
- Total homepage weight under 500KB
- No external font CDN calls
- Reserve space for all images before they load to prevent CLS

---

## 2. SCHEMA MARKUP — UPDATED FOR MARCH/MAY 2026

Use **JSON-LD only**. Place in `<head>`.

### What's still active and valuable in 2026:
- ✅ AccountingService / LocalBusiness — critical for map pack and AI answers
- ✅ Person schema — for Mike's bio page
- ✅ BreadcrumbList — for site hierarchy
- ✅ Service schema — for individual service pages
- ✅ FAQPage — for AI citation only (NOT Google rich results anymore)
- ✅ Organization — sitewide in header/footer
- ❌ HowTo — no longer generates rich results (inert but not harmful)

### Primary Schema: AccountingService

```json
{
  "@context": "https://schema.org",
  "@type": "AccountingService",
  "name": "Rank 1 Accounting",
  "url": "https://rank1accounting.com",
  "logo": "https://rank1accounting.com/logo.png",
  "image": "https://rank1accounting.com/office-photo.jpg",
  "description": "Rank 1 Accounting provides bookkeeping, tax planning, payroll, sales tax, and advanced tax minimization strategies for business owners and high-income earners in Staten Island and New York City.",
  "telephone": "+1-[PHONE]",
  "email": "[EMAIL]",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "[STREET ADDRESS]",
    "addressLocality": "Staten Island",
    "addressRegion": "NY",
    "postalCode": "[ZIP]",
    "addressCountry": "US"
  },
  "geo": {
    "@type": "GeoCoordinates",
    "latitude": "[LAT]",
    "longitude": "[LONG]"
  },
  "areaServed": [
    {"@type": "City", "name": "Staten Island"},
    {"@type": "City", "name": "New York City"},
    {"@type": "AdministrativeArea", "name": "Hamptons"},
    {"@type": "State", "name": "New York"}
  ],
  "openingHoursSpecification": [
    {
      "@type": "OpeningHoursSpecification",
      "dayOfWeek": ["Monday","Tuesday","Wednesday","Thursday","Friday"],
      "opens": "09:00",
      "closes": "17:00"
    }
  ],
  "priceRange": "$$",
  "hasOfferCatalog": {
    "@type": "OfferCatalog",
    "name": "Accounting Services",
    "itemListElement": [
      {"@type": "Offer", "itemOffered": {"@type": "Service", "name": "Bookkeeping Services"}},
      {"@type": "Offer", "itemOffered": {"@type": "Service", "name": "Individual Tax Planning"}},
      {"@type": "Offer", "itemOffered": {"@type": "Service", "name": "Corporate Tax Services"}},
      {"@type": "Offer", "itemOffered": {"@type": "Service", "name": "Quarterly Tax Filings"}},
      {"@type": "Offer", "itemOffered": {"@type": "Service", "name": "Sales Tax Filing"}},
      {"@type": "Offer", "itemOffered": {"@type": "Service", "name": "Payroll Services"}},
      {"@type": "Offer", "itemOffered": {"@type": "Service", "name": "Real Estate Accounting"}},
      {"@type": "Offer", "itemOffered": {"@type": "Service", "name": "Wealth Management"}},
      {"@type": "Offer", "itemOffered": {"@type": "Service", "name": "Trust and Estate Planning"}},
      {"@type": "Offer", "itemOffered": {"@type": "Service", "name": "Tax Minimization Strategy"}}
    ]
  },
  "founder": {
    "@type": "Person",
    "name": "Michael McEvoy",
    "jobTitle": "CPA",
    "url": "https://rank1accounting.com/about"
  },
  "sameAs": [
    "https://www.google.com/maps/[GBP_LINK]",
    "https://www.yelp.com/biz/[YELP_LINK]",
    "https://nysscpa.org/[PROFILE]"
  ]
}
```

### IMPORTANT Schema Rule (March 2026):
Every field in schema must EXACTLY match what's visible on the page AND your Google Business Profile. Phone format, address format — identical everywhere. Mismatches reduce trust signals.

---

## 3. KEYWORD INTELLIGENCE

### Primary target keywords by funnel:

**Funnel 2 — Bookkeeping/Business (high search volume, local intent):**
- "CPA Staten Island" — primary, high intent
- "accountant Staten Island NY" 
- "bookkeeping services Staten Island"
- "small business accountant Staten Island"
- "tax preparation Staten Island"
- "sales tax filing NYC"
- "bookkeeper Brooklyn NY"
- "small business CPA NYC"
- "quarterly tax filing New York"
- "payroll services Staten Island"
- "IRS notice help NYC"
- "bookkeeping for contractors Staten Island"
- "restaurant bookkeeping NYC"
- "accounting services for small business NYC"

**Funnel 3 — Tax Savings/Wealthy (lower volume, higher value):**
- "tax planning high income New York"
- "tax minimization strategies NYC"
- "CPA for high earners New York"
- "advanced tax planning Hamptons"
- "tax savings wealthy individuals NYC"
- "real estate investor tax planning NYC"
- "physician tax planning New York"
- "how to reduce taxes legally New York"
- "tax write offs for business owners NYC"
- "vehicle tax deduction New York business"
- "wealth management CPA Staten Island"
- "trust and estate tax planning NYC"

**AEO/Voice/AI Search queries to target in FAQ content:**
- "how do I save money on taxes in New York"
- "can I write off my car as a business expense in New York"
- "what can a small business write off in NYC"
- "how to find a CPA in Staten Island"
- "what does a bookkeeper cost in Staten Island"
- "how to respond to an IRS notice in New York"
- "best accountant for high earners in New York"
- "how much does tax preparation cost in NYC"
- "what is the sales tax rate in New York City"
- "do I need a CPA for my small business in NYC"

**Key insight from competitor research:**
NYC has extremely high combined tax burden (federal + state 10.90% + NYC 3.876% = nearly 50% for high earners). This is a massive pain point. The angle "New York takes nearly half your income — we help you keep more" is powerful and underused.

---

## 4. COMPETITOR LANDSCAPE (Staten Island)

Top competitors found:
- **Roman & Associates CPA** — romankcpa.com — Staten Island, established firm
- **Aqua Tax & Accounting** — aquataxaccounting.com — Staten Island, 189 Main St
- **Dimov Tax** — dimovtax.com — has a Staten Island landing page, aggressive SEO

**Gaps to exploit:**
- None of them lead with tax minimization/savings angle
- None target wealthy individuals specifically
- None have dedicated Hamptons/Upper East Side pages
- Their websites are outdated — Rank 1 can look dramatically more premium
- Bookkeeping pricing in Staten Island: $400-$800/mo part-time, $3,000-$4,500 full-time — use this for pricing context

---

## 5. E-E-A-T FOR FINANCIAL/TAX SITES (YMYL Category)

Google treats accounting/tax as YMYL (Your Money or Your Life) — highest scrutiny.

**Must have on the website:**
- Mike's full name + CPA credential + license number visible
- Years of experience stated explicitly
- Real photo of Mike — not stock photos
- Physical address — real, verifiable
- Real phone number — click to call on mobile
- Privacy policy page
- Disclaimer: "This content is for informational purposes. Consult a CPA for advice specific to your situation."
- Google Reviews widget or count displayed
- NYSSCPA member listing linked
- BBB accreditation if applicable

---

## 6. AEO — UPDATED FOR 2026

**Key stats:**
- Google AI Overviews appear on 25.8% of financial services searches
- AI search visitors convert at 4.4x rate of traditional organic visitors
- Only 12% of URLs cited by ChatGPT rank in Google's top 10 — meaning AI citation and Google ranking are separate games

**How each AI engine cites:**
- **ChatGPT:** Favors authoritative long-form content with clear structure
- **Perplexity:** Favors fresh, well-cited content — update pages regularly, add "Last updated" dates
- **Google AI Overviews:** Favors pages already ranking top 10 + structured data
- **Voice/Siri/Alexa:** Favors short direct answers, local business schema, GBP data

**AEO content rules:**
- Every page leads with a direct 50-80 word answer to its main question
- FAQ sections with questions phrased exactly how someone asks their phone
- Short paragraphs — max 3 sentences
- Use entity-based content: IRS, New York State, QuickBooks, W-2, 1099, Schedule C, LLC, S-Corp
- Cite authoritative sources in content: IRS.gov, nysscpa.org, tax.ny.gov
- Add "Last updated: [date]" to all key pages

---

## 7. LOCAL SEO SIGNALS

- NAP must be IDENTICAL everywhere: website, GBP, Yelp, BBB, NYSSCPA directory
- Include full address in text on every page — not just footer
- H1 must include service + location on every page
- Mention Staten Island neighborhood names naturally in content
- Get reviews with location keywords in them
- Post to Google Business Profile weekly
- Get listed on: Google Business Profile, Yelp, BBB, NYSSCPA, Thumbtack, Angi

---

## 8. PAGE SPEED — TECHNICAL RULES

Target: Under 1 second LCP desktop, under 2 seconds mobile.

```html
<!-- System font stack — no external fonts needed -->
<style>
  body { font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif; }
</style>

<!-- Preload hero image -->
<link rel="preload" as="image" href="/hero.webp" fetchpriority="high">

<!-- Hero image implementation -->
<img src="/hero.webp" alt="Rank 1 Accounting Staten Island CPA" 
     width="1200" height="600" fetchpriority="high">

<!-- Below fold images -->
<img src="/service.webp" alt="Tax planning services" 
     width="600" height="400" loading="lazy">
```

---

## 9. TITLE TAGS & META DESCRIPTIONS

**Homepage:**
- Title: `CPA & Tax Planning Services in Staten Island, NY | Rank 1 Accounting`
- Meta: `Rank 1 Accounting helps business owners and high earners in Staten Island legally reduce taxes, manage bookkeeping, and plan for financial success. Book a free consultation.`

**Per landing page format:**
- Title: `[Service] in [Location] | Rank 1 Accounting`
- Meta: `Rank 1 Accounting provides [service] for [audience] in [location]. [Key benefit]. Book a free consultation today.`

Title max: 60 characters. Meta max: 160 characters. Every page unique.

---

## 10. LANDING PAGE PRIORITY ORDER

**Build in this exact order:**

1. Homepage (most important — do this first, do it perfectly)
2. Bookkeeping for contractors — Staten Island
3. Tax planning for high earners — New York
4. CPA services — Brooklyn
5. Tax savings — Hamptons NY
6. Bookkeeping for restaurants — NYC
7. Real estate investor tax planning — NYC
8. Physician tax planning — New York
9. Sales tax filing — NYC
10. Payroll services — Staten Island

---

## 11. CONTENT RULES — NON-NEGOTIABLE

- NO em dashes anywhere
- NO AI-sounding phrases
- NO generic claims like "committed to excellence"
- Short sentences, short paragraphs
- "You" and "your" — write to the reader directly
- Every page needs FAQ section (for AI citation)
- All FAQ answers: 40-80 words, complete and direct
- Use location name naturally 3-4 times per landing page
- Lead with pain point, not credentials

---

## 12. FINAL CHECKLIST BEFORE SHIPPING ANY PAGE

- [ ] LCP image has `fetchpriority="high"` and is preloaded
- [ ] All images have explicit width/height and WebP format  
- [ ] No render-blocking CSS or JS
- [ ] System fonts only
- [ ] AccountingService JSON-LD schema in `<head>`
- [ ] FAQPage JSON-LD schema (for AI citation, not Google rich results)
- [ ] BreadcrumbList schema
- [ ] H1 includes service + location
- [ ] Title tag 50-60 chars
- [ ] Meta description 150-160 chars
- [ ] FAQ section visible on page
- [ ] Mike's CPA credentials visible
- [ ] Real address and phone in page text
- [ ] No em dashes
- [ ] Booking button above the fold
- [ ] Click-to-call phone on mobile
- [ ] Page weight under 500KB
- [ ] "Last updated" date on page

---

*Research compiled and updated June 9, 2026*
*Key correction: FAQPage schema no longer generates Google rich results as of May 7, 2026*
*Sources: Google Search Central, Schema.org v30.0, W3Era, DigitalApplied, Conductor AEO Benchmarks*
