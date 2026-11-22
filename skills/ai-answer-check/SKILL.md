---
name: ai-answer-check
description: Check whether ChatGPT, Gemini, Claude and Perplexity name a local business when asked for recommendations in its city, and which sources they cite. Use when a local business asks "does AI recommend us?" or wants a baseline before and after fixes.
---

# AI answer check for a local business

AI assistants often name different businesses for the same question, and they mostly cite third-party pages (lists, articles, directories) rather than the business's own site. Check several assistants and several phrasings before drawing conclusions.

## Inputs to ask for
- Business name, main service, city or neighborhood.
- 2 or 3 competitors the owner thinks of as rivals (optional).

## Build the prompts (6 to 10)
Mix these types:
- Category: "Who's the best [service] in [city]?"
- Specific service: "Who does [specific job] in [city]?" (for example "same-day water heater repair")
- Customer need: "Where can I get [need] near [neighborhood]?" (for example "a quiet haircut", "a dentist open Saturday")
- Comparison: "[Business] vs [competitor]: which is better for [need]?"
- Direct: "What do you know about [business name] in [city]?"

## Steps
1. Ask each prompt in each assistant you have access to. Use a fresh chat with no prior context. If you can only reach some assistants, say which ones you skipped.
2. For each answer, record:
   - Whether the business is named, and its position in the list
   - The other businesses named
   - The cited sources or links (domain and type: list/article, directory/review site, business website, Reddit, news)
3. Run the full set twice if possible. Answers vary between runs, so look for patterns, not a single result.

## Output
1. A score: named in X of Y answers, broken down by assistant.
2. The competitors named most often.
3. The source domains cited most often, grouped by type. These are where the business needs to appear.
4. The top 3 actions. Usually: get onto the most-cited list or directory pages, fix missing or inconsistent listings (`nap-consistency`), and add the missing service or FAQ content to the website (`local-site-basics`).

## Rules
- Report what the assistants said. Don't claim a guaranteed fix: AI answers change over time.
- Save the prompts so the owner can rerun the same set in a few weeks.
