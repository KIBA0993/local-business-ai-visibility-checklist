---
name: gbp-audit
description: Audit a local business's Google Business Profile against the top 3 competitors on Google Maps and produce a prioritized fix list. Use when someone asks why they don't show up on Google Maps, or wants to improve a new GBP.
---

# Google Business Profile audit

Goal: a short, prioritized list of fixes for one Google Business Profile (GBP), based on what the businesses that already rank are doing.

## Inputs to ask for
- Business name, city or neighborhood, and main service (for example "emergency plumber", "nail salon").
- The GBP link, or permission to look it up.

## Steps
1. **Find the competition.** Search Google Maps for "[main service] near [city]". Note the top 3 businesses in the local pack. Skip the business being audited if it already appears.
2. **Collect the same fields for the business and each competitor:**
   - Primary category and secondary categories
   - Number of reviews, average rating, and newest review date
   - Number of photos, and whether there are photos of the outside, inside, team and work
   - Whether services/products are listed, with descriptions
   - Whether the description mentions the service and city
   - Hours, website link, booking link, phone
   - Posts in the last 30 days
3. **Compare.** Put the results in one table with a column per business.
4. **Write the fix list,** most impactful first:
   - Primary category: pick the most specific category that is true for the business. Copy a competitor's category only if it accurately describes the business.
   - Missing secondary categories that genuinely apply.
   - Missing services, each with a one-sentence description (what, who for, rough price).
   - Photos: target at least 10 real photos covering outside, inside, team and work.
   - Review gap: the number of reviews needed to reach the median of the top 3, and a realistic weekly target.
   - Anything inconsistent (hours, phone, website) with other listings. Hand off to the `nap-consistency` skill.

## Rules
- Never suggest fake reviews, review gating, keyword-stuffing the business name, or a virtual office address. These violate Google's guidelines and can get the profile suspended.
- New profiles may still be in verification. If so, say that the fixes apply once verification completes.

## Output
A comparison table, then a numbered fix list with an estimated effort for each item (5 min / 30 min / ongoing).
