---
name: local-site-basics
description: Check and fix the website basics that help a local business get found by Google and AI assistants, covering service and area pages, FAQ, LocalBusiness schema, AI crawler access in robots.txt, and mobile tap-to-call. Use on a local business website or its codebase.
---

# Local website basics

A Seeably study of 6,682 US local businesses found that 17.5% of businesses with a website were named by at least one of four AI assistants, against 4.4% of those without one. The site doesn't need to be fancy. It needs to say clearly what the business does, where, and for whom.

## Inputs
- Website URL, or the site's codebase if you're working in it.
- List of services and service areas, from the owner.

## Checks
1. **Service pages.** Each main service has its own page, with the service and city in the title and H1. Flag services that only appear in a bullet list on the home page.
2. **Area pages.** If the business serves several towns or neighborhoods, each main area has a page with genuinely local details (not the same text with the city name swapped).
3. **FAQ.** Answers to the questions customers ask on the phone: price ranges, timing, what to expect, parking, payment, insurance. Draft missing answers with the owner and use their facts.
4. **LocalBusiness schema.** JSON-LD with the most specific type (for example `Plumber`, `HairSalon`, `Dentist`), plus name, address, phone, URL, opening hours, geo, `areaServed`, and `sameAs` links to the Google, Yelp, Apple and Facebook profiles. Check that it validates (validator.schema.org).
5. **NAP match.** The name, address and phone on the site match the Google Business Profile exactly.
6. **robots.txt.** Check it doesn't block AI crawlers (GPTBot, OAI-SearchBot, ClaudeBot, PerplexityBot, Google-Extended) unless the owner wants to block them. Point out that blocking them can keep the business out of AI answers.
7. **Mobile.** A tap-to-call phone link (`tel:`) and the booking button are visible at the top of the page on a phone.
8. **Basics.** Each page has a unique title and meta description, pages load on mobile, and there are no broken links to the booking tool or the map.

## Output
A pass/fail table for the checks above. Then concrete fixes: if you have the codebase, make the changes directly (schema, pages, robots.txt). Otherwise give the exact text and code to paste.

## Rules
- Don't invent services, prices, awards or reviews. Ask the owner.
- Don't create thin doorway pages for towns the business doesn't actually serve.
