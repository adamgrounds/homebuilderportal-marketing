# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Status

**Pre-development.** The only file currently in this repository is `HomeBuilderPortal-Marketing-Website-PRD.md`. No framework, build tooling, or code exists yet. When a framework is chosen, update this file with build/dev/test commands.

## What This Project Is

A B2B marketing website for **Home Builder Portal** — a SaaS platform that helps home builder companies communicate with homebuyers during construction. The marketing site's sole conversion goal is driving **demo requests**.

## Open Decisions That Must Be Resolved Before Development

These are blocking (from the PRD):
1. **Framework/CMS** — Next.js + headless CMS, Astro, Webflow, etc. (affects speed targets and SEM page deployment)
2. **CRM** — HubSpot or equivalent (affects demo form integration)
3. **Brand assets** — Logo, colors, and typography must be finalized before design begins
4. **Domain** — Root domain vs. subdomain; hosting configuration

## Site Architecture

| Route | Purpose | Priority |
|---|---|---|
| `/` | Homepage | P0 — Launch |
| `/demo` | Demo request form page | P0 — Launch |
| `/thank-you` | Post-submission confirmation | P0 — Launch |
| `/leaders` | SEM landing page (executive persona) | P0 — Launch |
| `/sales-managers` | SEM landing page (sales manager persona) | P0 — Launch |
| `/privacy-policy` | Legal | P0 — Launch |
| `/terms-of-service` | Legal | P0 — Launch |
| `/features` | Full feature list | P1 |
| `/blog` | SEO content hub | P2 — Post-Launch |
| `/case-studies` | Customer proof | P2 — Post-Launch |

## Two Target Personas

All copy and page structure must serve both of these:

- **Builder Executive** — Cares about brand, competitive differentiation, ROI, referrals, and reviews
- **Sales Manager** — Cares about reducing inbound buyer interruptions and improving sales metrics

Persona-specific landing pages (`/leaders`, `/sales-managers`) are P0 SEM pages with no navigation and a single embedded CTA.

## Performance Requirements (Non-Negotiable)

- Google PageSpeed Insights 90+ on both mobile and desktop
- Core Web Vitals: LCP < 2.5s, CLS < 0.1, INP < 200ms
- All images in WebP format with lazy loading and alt text
- Mobile-first, responsive layout

## SEO Technical Checklist (Every Page)

- Unique H1 targeting the page's primary keyword
- Meta title: 50–60 characters
- Meta description: 150–160 characters with CTA language
- Open Graph tags for social sharing
- Canonical URLs on all pages
- XML sitemap auto-generated and submitted to Google Search Console
- `robots.txt` allowing all public pages
- HTTPS enforced

## Analytics Requirements

- GA4 with conversion events: demo form view, demo form submission, CTA button clicks
- Google Tag Manager container for tag management without code deploys
- Google Search Console verified with sitemap submitted

## Demo Request Form Fields

First name, last name, company name, email, phone (optional), homes per year (dropdown). Submission must trigger a confirmation email and route to CRM.

## Key Messaging Reference

Full messaging pillars are in the PRD appendix. Core themes:
- For executives: buyer experience during construction drives referrals, reviews, and repeat business
- For sales managers: less reactive communication = more time selling; informed buyers = good reviews
- Platform differentiators: branded portal, field updates in under a minute, message templates, public share links
