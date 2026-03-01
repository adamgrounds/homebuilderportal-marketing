# Home Builder Portal
## Marketing Website — Product Requirements Document (PRD)

| Field | Value |
|---|---|
| **Status** | Draft |
| **Version** | 1.0 |
| **Date** | March 2026 |
| **Owner** | [Product Owner TBD] |
| **Stakeholders** | Executive Leadership, Sales Team, Engineering, Marketing |

---

## Table of Contents

1. [Overview](#1-overview)
2. [Problem Statement](#2-problem-statement)
3. [Goals](#3-goals)
4. [Non-Goals](#4-non-goals)
5. [Target Audience](#5-target-audience)
6. [User Stories](#6-user-stories)
7. [Requirements](#7-requirements)
8. [SEO & SEM Strategy](#8-seo--sem-strategy)
9. [Site Architecture](#9-site-architecture)
10. [Success Metrics](#10-success-metrics)
11. [Open Questions](#11-open-questions)
12. [Timeline Considerations](#12-timeline-considerations)
13. [Appendix: Key Messaging Reference](#appendix-key-messaging-reference)

---

## 1. Overview

Home Builder Portal is a branded, mobile-first communication platform that keeps homebuyers informed, excited, and engaged throughout the construction process. This PRD covers the requirements for the public marketing website that will attract, educate, and convert home builder companies into demo requests and customers.

---

## 2. Problem Statement

Home builder companies lack a modern, branded way to communicate with homebuyers during construction. Buyers are left in the dark, generating a flood of inbound calls and emails to sales teams and site superintendents. This erodes buyer confidence, hurts reviews, and reduces referrals.

Home Builder Portal solves this with a platform that lets builders post field updates in under a minute — using templates for consistency — while giving buyers a polished, branded portal to track their home's progress in real time.

The marketing website must clearly communicate this value to two primary decision-maker personas — builder executives focused on brand and ROI, and sales managers focused on efficiency and reviews — and drive them toward booking a demo.

---

## 3. Goals

- Drive demo requests as the primary conversion action, targeting a minimum **3% visitor-to-demo conversion rate** within 90 days of launch.
- Rank on the first page of Google for target keywords (e.g., "homebuilder buyer portal," "construction communication platform") **within 6 months** of launch.
- Achieve a **Google PageSpeed Insights score of 90+** on mobile and desktop to support both SEO rankings and user experience.
- Clearly communicate the two-sided value of the platform (for builder teams and for buyers), reducing friction for both executive and sales manager personas.
- Support SEM campaigns with purpose-built landing pages that can be deployed quickly for paid search and paid social ad groups.

---

## 4. Non-Goals

- **Self-serve signup or account creation:** The marketing site will not include in-product signup flows. All conversions route to a demo request. Self-serve onboarding is a future initiative.
- **Full product documentation or knowledge base:** A separate help center will be built later. The marketing site focuses on acquisition, not support.
- **Blog or content marketing hub (Phase 1):** A blog may be added in Phase 2 as an SEO content engine, but it is out of scope for the initial launch.
- **Buyer-facing marketing:** This site targets home builder companies (B2B), not end homebuyers. Buyer-facing content or flows are out of scope.
- **E-commerce or payment functionality:** No pricing pages with self-serve checkout. Pricing will be discussed during the demo.

---

## 5. Target Audience

The marketing website serves two primary decision-maker personas within home builder companies:

### 5.1 Builder Executive (Economic Buyer)

Cares about brand, competitive differentiation, and return on investment. Responds to: positioning against competitors still using email threads and PDF attachments; the connection between buyer experience during construction and 5-star reviews, referrals, and repeat business; and platform scalability from a single community to hundreds of homes.

### 5.2 Sales Manager (Champion / End User)

Cares about reducing inbound buyer interruptions and improving their sales metrics. Responds to: posting a photo or video update in under a minute directly from the job site; pre-built message templates ensuring consistent, polished buyer communication; and the direct link between informed buyers, better reviews, and more referrals during construction — not just after closing.

---

## 6. User Stories

### 6.1 Prospective Customer (Site Visitor)

- As a **builder executive** visiting the site, I want to immediately understand what Home Builder Portal does and how it differentiates my company, so that I can decide whether to book a demo.
- As a **sales manager** visiting the site, I want to see a concrete before-and-after of what my day would look like using the platform, so that I can advocate for it internally.
- As **any visitor**, I want the site to load instantly on my phone, so that I don't abandon it before understanding the product.
- As a **visitor arriving from a Google ad**, I want a landing page that matches my search intent and has a single clear call-to-action, so that I can take the next step without confusion.

### 6.2 Marketing & Sales Team (Internal User)

- As a **marketer**, I want to deploy new SEM landing pages quickly without engineering involvement, so that I can test ad campaigns efficiently.
- As a **sales rep**, I want a link to send prospects that clearly shows the product's value, so that I can support outbound sales conversations.

---

## 7. Requirements

### 7.1 Must-Have — P0 (Launch Blockers)

#### Homepage

The homepage is the primary entry point for both organic and paid traffic.

- **Hero section** with a clear headline communicating the core value proposition (e.g., "Keep your homebuyers informed — without adding work to your team"), a short subheadline, and a prominent "Book a Demo" CTA button.
- **Two-sided value section:** a visual split between "For your team" and "For your buyers", mirroring the dual-persona messaging from the sales materials.
- **Feature highlight section** covering: branded buyer portal, field photo/video posting, message templates, file vault, public share links, and multi-home management.
- **Social proof section** (testimonials placeholder at launch; real quotes populated post-launch).
- **Final CTA section** with demo request form embedded or linked.

#### Demo Request Flow

- A demo request form collecting: first name, last name, company name, email address, phone number (optional), number of homes per year (dropdown).
- Form submission triggers a confirmation email and routes to CRM (HubSpot or equivalent — TBD by engineering).
- A post-submission thank-you page confirming next steps.

#### Performance & SEO Technical Requirements

- Google PageSpeed Insights score of **90+** on both mobile and desktop.
- Core Web Vitals passing thresholds: LCP under 2.5s, CLS under 0.1, INP under 200ms.
- Fully responsive layout, mobile-first breakpoints.
- Semantic HTML5 structure with proper heading hierarchy (H1, H2, H3).
- Meta titles and meta descriptions set for all pages; Open Graph tags for social sharing.
- XML sitemap auto-generated and submitted to Google Search Console.
- `robots.txt` configured to allow crawling of all public pages.
- Canonical URLs set to prevent duplicate content issues.
- All images served in WebP format with lazy loading and descriptive alt text.
- HTTPS enforced site-wide with valid SSL certificate.

#### Analytics & Tracking

- Google Analytics 4 (GA4) installed and configured with conversion events for: demo form view, demo form submission, CTA button clicks.
- Google Tag Manager (GTM) container deployed for flexible tag management without code deploys.
- Google Search Console verified and sitemap submitted.

---

### 7.2 Nice-to-Have — P1 (Target for Launch)

- **Persona-specific landing pages:** a version of the homepage optimized for the "Builder Executive" angle and one for the "Sales Manager" angle, suitable for targeted SEM ad groups.
- An **animated or interactive product demo section** (e.g., a short auto-playing video or a screenshot carousel) showing the field posting and buyer portal experience.
- A simple **FAQ section** addressing common objections: pricing, implementation time, mobile compatibility, and integration with existing systems.
- **Structured data markup** (Schema.org `SoftwareApplication` or `Organization`) to support rich snippets in Google search results.
- A **"How It Works" section** with a numbered 3-step visual flow for both the builder team and the buyer.

---

### 7.3 Future Considerations — P2 (Post-Launch)

- Blog / content marketing hub for long-tail SEO content targeting homebuilder industry keywords.
- Case studies page with named customer logos and quantified results (e.g., "40% reduction in inbound buyer calls").
- Pricing page (when pricing strategy is finalized and self-serve or transparent pricing is adopted).
- Live chat widget (e.g., Intercom or Drift) for real-time engagement with high-intent visitors.
- A/B testing framework on hero headlines and CTA copy to optimize conversion rate.

---

## 8. SEO & SEM Strategy

### 8.1 Target Keywords

| Keyword / Theme | Intent | Target Page |
|---|---|---|
| homebuilder buyer portal | Commercial | Homepage |
| construction update software for builders | Commercial | Homepage |
| home builder communication platform | Commercial | Homepage |
| keep homebuyers informed during construction | Informational | How It Works / Blog (P2) |
| reduce buyer calls during construction | Problem-Aware | Sales Manager Landing Page |
| homebuilder customer experience software | Commercial | Homepage |
| new home construction tracker for buyers | Informational | Homepage / Blog (P2) |

### 8.2 SEM Landing Pages

Paid search and paid social campaigns require dedicated landing pages with:

- Headline and copy that directly matches the ad's message (message match).
- A single CTA — no navigation menu or secondary links to reduce distraction.
- A short-form demo request embedded above the fold.
- The relevant persona angle: executive-focused or sales-manager-focused depending on the ad group.

### 8.3 On-Page SEO Checklist (Per Page)

- Unique, keyword-targeted H1 on every page.
- Meta title: 50–60 characters, includes primary keyword.
- Meta description: 150–160 characters, includes CTA language.
- Internal linking between pages (homepage → how it works, features, demo).
- External links to authoritative sources where relevant (nofollow where appropriate).

---

## 9. Site Architecture

| Page | Purpose | Priority |
|---|---|---|
| `/` | Main homepage, primary organic and direct traffic destination | P0 — Launch |
| `/demo` | Demo request page with embedded form | P0 — Launch |
| `/thank-you` | Post-submission confirmation page | P0 — Launch |
| `/features` | Full feature list with detail | P1 |
| `/leaders` | Persona-specific SEM landing page | P0 - Launch |
| `/sales-managers` | Persona-specific SEM landing page | P0 - Launch |
| `/privacy-policy` | Legal requirement | P0 — Launch |
| `/terms-of-service` | Legal requirement | P0 — Launch |
| `/blog` | SEO content hub | P2 — Post-Launch |
| `/case-studies` | Customer proof | P2 — Post-Launch |

---

## 10. Success Metrics

### 10.1 Leading Indicators (First 30 Days Post-Launch)

- **PageSpeed Insights score:** 90+ on mobile and desktop.
- **Google Search Console:** site indexed within 7 days of launch; zero crawl errors.
- **Demo form submission rate:** tracked in GA4 from day one.
- **SEM Quality Score:** landing pages achieve Google Ads quality score of 7+ for target ad groups.

### 10.2 Lagging Indicators (90 Days Post-Launch)

- **Organic keyword rankings:** at least 3 target keywords on page 1 of Google within 6 months.
- **Demo conversion rate:** 3%+ of unique visitors submit a demo request.
- **Organic traffic growth:** month-over-month increase in organic sessions.
- **Bounce rate:** under 60% on the homepage for organic and direct traffic.
- **Demo-to-pipeline rate:** tracked in CRM — percentage of demo requests that convert to qualified opportunities (target TBD with sales team).

---

## 11. Open Questions

| Question | Owner | Priority |
|---|---|---|
| Which CMS or framework will be used? (e.g., Next.js + headless CMS, Webflow, etc.) This affects speed targets, SEM page deployment flexibility, and engineering lift. | Engineering | High |
| Which CRM will capture demo form submissions? Integration requirements will affect form build. | Sales / Ops | High |
| Do we have existing brand assets (logo, brand colors, typography)? If not, design work is needed before development begins. | Design / Marketing | High |
| What is the primary domain? Is the marketing site a subdomain or the root domain? | Engineering / Marketing | High |
| Do we have any existing customer testimonials or case study data we can use at launch, or will social proof be placeholder? | Sales | Medium |
| Is there a product video or screen recording available to embed, or does one need to be produced? | Marketing / Design | Medium |
| Are there legal/compliance requirements around the demo request form (e.g., GDPR consent for any EU prospects)? | Legal | Medium |

---

## 12. Timeline Considerations

| Phase | Scope | Suggested Timeline |
|---|---|---|
| **Phase 1: Foundation** | Homepage, `/demo`, `/thank-you`, privacy/terms. Full P0 requirements including SEO technical setup, GA4, GTM. | Weeks 1–4 |
| **Phase 2: Conversion Optimization** | Persona landing pages, `/features` page, product video embed, FAQ section. | Weeks 5–8 |
| **Phase 3: SEO Scaling** | Blog / content hub, case studies, structured data, A/B testing framework. | Weeks 9+ |

**Hard dependencies:** Brand assets (logo, colors, typography) must be finalized before design begins. CRM integration must be confirmed before form development begins. Domain and hosting must be configured before QA and launch.

---

## Appendix: Key Messaging Reference

The following messaging pillars are drawn directly from the executive and sales manager pitch materials and should inform copywriting across all pages.

### For Builder Executives

- "Homebuyers are making the largest purchase of their lives — and during construction, they're often in the dark."
- "The experience your buyer has during construction is the one they remember. It shapes referrals, reviews, and repeat business."
- "The best builders tirelessly focus on providing the best customer experience. This is a clear opportunity to shine."
- "Buyers' expectations are high and are set by the best consumer apps they use every day. They tap a button and have dinner dropped on their porch. They obsessively seek out the best reviewed restaurants before making a reservation. Creating a good customer experience is critical to your business and Home Builder Portal helps you stand out from the crowd."

### For Sales Managers

- "Your buyers go quiet after contract — and that's a problem."
- "Less time reactively communicating means more time selling."
- "Happy buyers write good reviews. Informed buyers are happy buyers."
- "Your best referral source isn't a past closing. It's a buyer in the middle of construction who can't stop showing people their new home under construction."

### Platform Differentiators

- Branded portal — buyers see the builder's logo and colors, not a generic tool.
- Mobile-first, app-like experience — works on any device, no app store required.
- Field updates posted in under a minute — photos, videos, captions.
- Message templates for consistent, on-brand communication across the entire team.
- Public share links — buyers share construction progress with family and friends, generating organic word-of-mouth.
- Scales from a single community to hundreds of homes on one dashboard.
