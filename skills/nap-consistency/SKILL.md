---
name: nap-consistency
description: Check that a local business's name, address, phone, website and hours match across Google, Apple Maps, Bing, Yelp and industry directories, and list exactly what to fix where. Use for new businesses, moves, phone changes or rebrands.
---

# NAP consistency check

NAP = Name, Address, Phone. AI assistants and maps apps cross-check these between sources. Mismatches make a business look less trustworthy, or like two different businesses.

## Inputs to ask for
- The correct, official name, address, phone, website and hours. Treat these as the source of truth.
- Industry (to pick the right directories).

## Steps
1. **Core listings.** Look up the business on each of these and record the NAP, website and hours shown, or "not listed":
   - Google Business Profile
   - Apple Maps (Apple Business Connect: businessconnect.apple.com)
   - Bing Places (bing.com/forbusiness)
   - Yelp
   - Facebook page
2. **Industry directories.** Pick the 3 to 5 that fit the industry. Examples:
   - Home services: Angi, Thumbtack, Houzz, BBB, Nextdoor
   - Health: Healthgrades, Zocdoc, WebMD
   - Legal: Avvo, Justia, FindLaw
   - Food: OpenTable, TripAdvisor, DoorDash/Uber Eats pages
   - Beauty and wellness: Vagaro, Booksy, Fresha, StyleSeat
3. **Search for strays.** Search the business name with the old phone or old address (if any), and the name plus the city. Look for duplicates and outdated listings.
4. **Compare** every listing with the source of truth. Treat formatting differences ("Ste" vs "Suite") as fine. Flag real differences: a different phone, an old address, a wrong name, missing hours, or a broken website link.

## Output
A table with one row per listing and these columns: Listing | Status (correct / wrong / missing / duplicate) | What's wrong | Fix link.
Then a to-do list ordered as: Google, Apple, Bing, Yelp, then the rest.

## Rules
- Don't create listings or claim profiles for the owner. Give them the links and the exact text to paste.
- Don't recommend paid citation-blast services. Fix the listings that matter by hand.
