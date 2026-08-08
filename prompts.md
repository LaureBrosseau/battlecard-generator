# The Prompts

In this file, you'll find **2 prompts**. The 1st one **generates the content of the battle card** and the second one **creates a HTML file** you can share as is or easily import in Canva or Notion.

---

## How to proceed

Use the first prompt, then check thoroughly the content generated.  
Fix inaccuracies if any and add/remove sections before generating the HTML file with the second prompt.

## Prompt 1: Generate the battle card content 

This is the prompt you can use to generate the content of the battle card.

1. Copy everything below into Claude or ChatGPT (or any other model of your choice).
2. Fill in the bracketed sections with your own raw data, and run it.
3. Handle the output as a first draft, **always fact-check before it goes to sales**.

---

```
You are helping me build a competitive battle card for my sales team, following a specific framework. Do not invent facts, pricing, or customer proof points — if something isn't in the material I give you, write "[NEEDS VERIFICATION]" instead of guessing.

## My company & product
Name: [Company name]
Find the location & founding: [City, Country · founded YYYY · public/private]
[Paste: 2-3 sentences on what your product does, your category claim, and your primary buyer persona]
Notable customer references: [a few notable customer references that the sales rep could share with the prospect]
Recent wins vs this competitor: [examples of recent wins against this specific competitor]
Useful resources for sales (2-3 links reps could use during a deal — e.g. G2/Capterra comparison page, official pricing page, internal competitive intel folder, win/loss call recordings, a customer story doc): [Paste your links here]

## Document ownership (for the footer)
Owner / team: [Name or team] Last updated: [use today's date, the date this battle card is generated] Next review: [today's date + 3 months, formatted as "Mon. YYYY", e.g. "Oct. 2026"]

## The competitor
Name: [Competitor name]
URL: [Competitor website URL]
Find the location & founding: [City, Country · founded YYYY · public/private]

Raw research (paste whatever you have: pricing page text, G2/Capterra review excerpts, changelog entries, call notes, LinkedIn posts, funding news):
[Paste raw material here]

## Instructions
Before writing anything, if either company's "Location & founding" field is left as a placeholder (not filled in), search the web yourself to find that company's headquarters city/country, founding year, and public/private status (including parent company ownership, e.g. "private, owned by [Parent Co.]"). Use official or primary sources where possible (company registries, the company's own site, press releases) over third-party aggregators, and note any discrepancy between sources if you find one. Only write "[NEEDS VERIFICATION]" for whatever you genuinely can't find after searching — don't ask me to fill these in myself.

Structure the battle card using exactly these 10 sections. Each one maps to a fixed slot in the HTML template — keep within the stated limits even if your source material has more nuance; anything that doesn't fit these limits should go in the "Gaps & extra context" note at the very end instead of being forced into a section.

1. **Snapshot**: three single sentences — who they are, why they win in some scenarios (honest), why we win in some scenarios (factual, not a knock). One sentence each, no more.

2. **Company & funding context**: about the competitor only, one short paragraph (2-3 sentences max). Only include if it's something that could truly change what a rep says or does (recent funding, layoffs, acquisition, leadership change). Otherwise write exactly "Nothing notable."

3. **Positioning comparison**: a 3-row table only — category claim, primary buyer, core promise — for them vs. me. One line per cell. Fold any nuance about whether this is a category/segment/feature fight into how you phrase these three rows rather than adding a separate explanatory line.

4. **Pricing & packaging**: pick ONE entry-tier price and ONE top/enterprise-tier price for each side (if a product has several tiers, choose the most representative entry and top tier; note any other tiers only inside the trap callout, don't add table rows for them). One line describing how each side's pricing scales ("growth model" row). Then a single consolidated callout (2-3 sentences max) naming the most important trap or friction point overall — not one trap per tier, just the single most decision-relevant one for a rep to flag.

5. **Capability comparison**: a table with exactly 3 columns — capability / them / me. Pick only 4-6 capabilities that are genuinely differentiated and likely to come up in real deals. Don't add a separate "so what" column — instead, fold the buyer implication directly and briefly into the "me" cell (e.g. "Native ATS with AI matching — buyers get X without a second tool" rather than a long explanation in a 4th column). Keep each cell to one short line.

6. **Where they win / where I win**: ONE short paragraph per side (2-3 sentences), organized around the single clearest use case or persona per side — not a bulleted list of multiple segments. Save specific customer names for section 9's customer-references slot, not here.

7. **Objection handling**: 3-5 real phrases a prospect would say, each with a short, honest response a rep can say out loud without sounding defensive. (This section repeats as a block per objection, so 5 is fine if you have 5 good ones.)

8. **Questions to ask (trap-setting questions)**: 3-5 discovery questions that surface their weak points naturally, without naming them. (Also a repeatable list, 5 is fine.)

9. **Proof points & customer references** — two short parts:
   - Proof points: 4-6 short, punchy stats or facts (not full sentences you'd read in a report — phrase each as a standalone one-liner under ~20 words), each with a source AND a date the fact was checked. Pick your strongest 4-6, don't dump every fact you have.
   - Customer references: one line per side listing publicly citable customer names (no descriptions needed, just names). If you have recent wins/losses against this competitor that aren't public info, flag them separately as "internal only — add manually" rather than writing them as if they were public proof points.

10. **Additional resources**: use the links I provided above, 2-4 of them. If I didn't provide any, suggest generic categories (G2/Capterra comparison, official pricing page) without inventing specific URLs.

Tone: direct, factual, respectful of the competitor. No marketing fluff, no unfair exaggeration of the competitor's weaknesses. A rep should be able to say any sentence in this out loud on a call without sounding either defensive or dishonest.

End with a short "Gaps to fill" list of anything you marked [NEEDS VERIFICATION], so I know exactly what to go research next.

## After the 10 sections, add one final block called "Gaps & extra context" — NOT part of the battle card itself, just for me:
- Every [NEEDS VERIFICATION] item, listed together, so I know exactly what to research next.
- Anything genuinely useful from the source material that didn't fit the format limits above (e.g. extra pricing tiers, extra personas, extra proof points) — summarized briefly so I don't lose it, but clearly marked as "left out of the template — for reference only."

```

Once your battle card content is created (using the prompt above), verify its content, pay also attention to content labelled "[NEEDS VERIFICATION]".  
Remove all content you cannot fact-check. You do not want to share with Sales false or inaccurate data.

Then once the content is ready, use the second prompt below. 

## Prompt 2: Turning your content into the HTML one-pager

This prompt will format your battle card content into a printable HTML template (battlecard-template.html). This content can be used on Canva or Notion.

Here's the prompt:

```
I have a battle card content (pasted below) and an HTML template (also pasted below). Fill the template with my content, keeping the HTML structure, CSS and layout exactly as they are — don't redesign anything, just replace the placeholder content with mine.

If my content doesn't fit a section cleanly (too long, missing information, extra information the template has no place for), tell me instead of forcing it in or cutting it silently.

## My battle card content
[Paste your finished, fact-checked battle card here]

## The HTML template
[Paste the full contents of battlecard-template.html here]

```

**What to do with the output**: copy the generated HTML, paste it into a plain text editor, and save the file with a .html extension.
Open it in a browser to check it, or if you'd rather work in a visual editor, import it into Canva (upload the HTML file, Canva converts it into an editable design).

:warning: Complex CSS and external fonts don't always survive the import perfectly, so expect to nudge colors or spacing afterward.

Once you have the battle card formatted, check the content (if not done yet) and the colors (green/orange). They should be used only on cells that are a true advantage for that company, not on frictions, limitations, or random numbers. Models get this wrong often enough that it's worth a real look, not a glance.

---

## Tips for better output

- **The quality of the battle card depends on the quality of your raw data.** Ten minutes on G2 reading actual customer complaints beats an hour of the model guessing from a category description.
- **Include call notes if you have any.** Real objections your reps have already heard are more valuable than anything on the competitor's own website.
- **Re-run it when something changes**: a pricing update, a new feature launch, a funding round. Paste the new information into the same prompt structure rather than starting from scratch.
- **Never skip the fact-check step.** The instruction to flag gaps helps, but models can still be confidently wrong about specifics like exact pricing tiers, verify anything a rep will say as fact.
