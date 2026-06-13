# Rank1CPA.com

Website for Rank1CPA — helping CPA firms achieve top search rankings.

## Skills installed

### SEO (`/seo`)
Full SEO suite — 25 sub-skills covering audits, technical SEO, content, local SEO, schema, sitemaps, backlinks, competitor analysis, and more.

| Command | Purpose |
|---------|---------|
| `/seo audit <url>` | Full site audit (up to 15 parallel agents) |
| `/seo page <url>` | Deep single-page analysis |
| `/seo technical <url>` | Technical SEO (9 categories) |
| `/seo content <url>` | E-E-A-T and content quality |
| `/seo local <url>` | Local SEO — GBP, citations, reviews, map pack |
| `/seo schema <url>` | Schema.org detection and generation |
| `/seo plan <type>` | Strategic SEO planning |
| `/seo cluster <keyword>` | Semantic topic clustering |
| `/seo backlinks <url>` | Backlink profile analysis |
| `/seo google [command] <url>` | Google APIs — GSC, PageSpeed, CrUX, GA4 |

### Design (`/nothing-design`)
Nothing-inspired UI/UX system — Swiss typography, monochromatic, information-dense.
Invoke with "Nothing style", "Nothing design", or `/nothing-design`.

### Claude Skills (345+ skills across 17 domains)
Available as `/cs-*` commands and agent personas. Key categories:
- **Engineering**: fullstack, frontend, backend, AI/ML, DevOps, security
- **Marketing**: SEO, ASO, content, demand gen, ads, funnels
- **C-Level Advisory**: CEO, CTO, CMO, CFO, COO, CPO advisors
- **Product**: roadmaps, OKRs, user stories, UX research
- **Research**: literature review, dossier, patent, pulse
- **Finance**: DCF valuation, budgeting, SaaS metrics
- **Compliance**: ISO 13485, GDPR, SOC2, FDA

## Stack

TBD — project in setup phase.


CLAUDE.md - Rank 1 CPA Website

Read this before touching anything. Every session. No exceptions.


THE PROJECT

Building rank1cpa.com - a national premium CPA firm website for Mike McEvoy.
This is a national brand. Not a local Staten Island site. Not a small tax office.
Think top Manhattan law firm competing nationally. That is the positioning. Always.

ABSOLUTE RULES - NEVER VIOLATE THESE

ZERO em dashes. Not in copy. Not in code. Not in comments. Not anywhere. Ever.
NO generic AI design. No purple gradients. No Inter font. No card layouts. No AI slop.
NO service list on the homepage body. Services live in nav dropdown and footer only.
NO FAQPage schema. Deprecated May 7 2026. Zero SERP value. Do not implement.
NO HowTo schema. Fully retired. Do not implement.
NO made up locations, services, or content. Only use what is explicitly provided.
NO em dashes. Repeating this because it keeps happening.

DESIGN SYSTEM

Use the Nothing Design skill loaded in this repo.

Direction: ultra premium, minimal, typographic, industrial luxury.
Feel: Blackstone Group meets Patek Philippe. Not H&R Block. Not a steakhouse.

Colors:


Background: near black - #0A0A0A
Primary gold accent: #C9A84C
Gold highlight: #F5E6A3
Gold shadow: #7A5C1E
Text: white or off-white only
Nothing else. No other colors.


Typography:


System fonts only. No Google Fonts. No external font CDN calls.
Bold, sharp, deliberate type treatment
Nothing generic


Motion:


Video hero background - full screen, dark overlay, loads AFTER LCP element
Scroll-triggered reveals - subtle, purposeful
No excessive animation. Less is more.


Performance:


Sub 1 second load time target
LCP under 2.5 seconds
INP under 200ms
CLS under 0.1
Mobile first. Always design mobile first.
All images WebP or AVIF format
Lazy load everything below the fold
Video never blocks LCP



HOMEPAGE STRUCTURE


Hero - full screen video background, dark overlay, one dominant headline, one CTA button
Authority section - brief, powerful, no fluff, no bullet points
Interactive tax savings calculator - this is the primary lead capture tool
Areas We Serve - subtle, small text, bottom of page only, not prominent


DO NOT add sections beyond this without being explicitly told to.


AREAS WE SERVE - FOOTER ONLY

These go at the very bottom. Small. Subtle. Not the focus of the page.
New York City, Brooklyn, Staten Island, Queens, The Hamptons

This is the launch territory. Do not add other cities unless told to.


SCHEMA MARKUP - JUNE 2026 GOOGLE STANDARDS

JSON-LD in the document head only. Schema.org v30.0. Every field must match visible page content exactly or Google penalizes.

Required on every page:


Organization - name, url, logo, sameAs linking to Google Business Profile and LinkedIn
LocalBusiness - name, address, telephone, geo coordinates, openingHoursSpecification
WebSite - with SearchAction
BreadcrumbList - on every single page
Person - for Mike McEvoy, with jobTitle, credentials, worksFor
ProfessionalService - serviceType, areaServed, provider


Validate everything against Google Rich Results Test standards before finalizing.


NAVIGATION


Logo top left
Nav links top right
Services in dropdown only - not listed on homepage body
One clear CTA button in nav - "Book a Consultation" or similar
Footer repeats nav links plus location list



COPY RULES


National positioning always. Never sound local or small.
Active voice. Short sentences. No fluff.
No em dashes. Using a regular hyphen or period instead if needed.
No exclamation points unless absolutely necessary.
Tone: authoritative, confident, premium. Not friendly and approachable.
Headlines: bold, direct, make a claim.



WHAT WE ARE NOT BUILDING


A template site
A local Staten Island CPA page
Anything that looks like it was built by AI
Anything generic
Anything with em dashes



TECH STACK


Pure HTML, CSS, JavaScript - no framework unless specifically requested
No jQuery
No unnecessary dependencies
Schema markup in JSON-LD script blocks in head
Sitemap.xml and robots.txt must be generated
All pages have canonical tags, OG tags, Twitter card tags
