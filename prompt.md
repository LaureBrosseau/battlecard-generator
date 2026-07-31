
# What you'll find here

In this file, you'll find **2 prompts**. The 1st one **generates the content of the battlecard** and the other **creates a HTML file** you can easily import in Canva or Notion.

## How to proceed

Use the first prompt, then check thoroughly the content generated.  
Fix inaccuracies if any and add/remove sections before generating the HTML file with the second prompt.

## Prompt 1: Generate the battlecard content 

This is the prompt you can use to generate the content of the battlecard.

1. Copy everything below into Claude or ChatGPT (or any other model of your choice).
2. Fill in the bracketed sections with your own raw data, and run it.
3. Handle the output as a first draft, **always fact-check before it goes to sales**.

---

```
You are helping me build a competitive battlecard for my sales team, following a specific framework. Do not invent facts, pricing, or customer proof points — if something isn't in the material I give you, write "[NEEDS VERIFICATION]" instead of guessing.

## My product
[Paste: 2-3 sentences on what your product does, your category claim, and your primary buyer persona]
Notable customer references: [a few notable customer references that the sales rep could share with the prospect]
Recent wins vs this competitor: [examples of recent wins against this specific competitor]

## The competitor
Name: [Competitor name]
URL: [Competitor website URL]

Raw research (paste whatever you have: pricing page text, G2/Capterra review excerpts, changelog entries, call notes, LinkedIn posts, funding news):
[Paste raw material here]

## Instructions
Structure the battlecard using exactly these 9 sections:

1. Snapshot: who they are (1 sentence), why they win in some scenarios (1 sentence, be honest), why they lose (1 sentence, be respectful, just fact)
2. Company & funding context: only include if there's something here that can truly influence the conversation (recent funding, layoffs, acquisition, leadership change). If nothing interesting, write "Nothing notable."
3. Positioning comparison: a table (category claim, primary buyer, core promise, for them vs. me), plus one line naming the real stake: is this a category disagreement, a segment disagreement, or a straight feature fight?
4. Pricing & packaging: entry price and what's actually included at that tier (not just the listed price, flag any traps in the tier limits), where their pricing model creates friction as the customer grows, where my model is genuinely better AND genuinely worse
5. Capability comparison: pick only 4-6 capabilities that are both genuinely differentiated and likely to come up in real deals. Table format: capability / them / me / one-sentence "so what" for the buyer
6. Where they win / where I win: segmented by use case or buyer persona, not by feature. Add a few customer references or recent wins if I've provided any.
7. Objection handling: 3-5 real phrases a prospect would say, each with a short, honest response, not something that sounds scripted, a real answer a rep can say out loud without sounding defensive
8. Trap-setting questions: discovery questions that surface their weak points naturally, without naming them
9. Proof points: pull only what's actually in the material provided. Mark anything unproven as "[NEEDS VERIFICATION]" rather than inventing a stat or quote, an unproven claim used on a call can damage the sales rep's and company's credibility, not build it.

Tone: direct, factual, respectful of the competitor. No marketing fluff, no unfair exaggeration of the competitor's weaknesses. A rep should be able to say any sentence in this out loud on a call without sounding either defensive or dishonest.

End with a short "Gaps to fill" list of anything you marked [NEEDS VERIFICATION], so I know exactly what to go research next.
```

## Prompt 2: Turning your content into the HTML one-pager

Once your battlecard content is drafted (using the prompt above) **and fact-checked**, use this second prompt to format it into a printable HTML template (battlecard-template.html). First verify the content thoroughly before generating the HTML template. Make sure content is trustful before it gets locked into a visual layout.  
Remove any content still labelled "[NEEDS VERIFICATION]" if you can't fact-check it — never hand Sales false or inaccurate data.  

Here's the prompt:

```
I have a fact-checked battlecard (pasted below) and an HTML template (also pasted below). Fill the template with my content, keeping the HTML structure, CSS and layout exactly as they are — don't redesign anything, just replace the placeholder content with mine.

If my content doesn't fit a section cleanly (too long, missing information, extra information the template has no place for), tell me instead of forcing it in or cutting it silently.

## My battlecard content
[Paste your finished, fact-checked battlecard here]

## The HTML template
[Paste the full contents of battlecard-template.html here]

```

**What to do with the output**: copy the generated HTML, paste it into a plain text editor, and save the file with a .html extension.   
Open it in a browser to check it before sharing, or if you'd rather work in a visual editor, import it into Canva (upload the HTML file, Canva converts it into an editable design).  
:warning: Complex CSS and external fonts don't always survive the import perfectly, so expect to nudge colors or spacing afterward. 


---

## Tips for better output

- **The quality of the battlecard depends on the quality of your raw data.** Ten minutes on G2 reading actual customer complaints beats an hour of the model guessing from a category description.
- **Include call notes if you have any.** Real objections your reps have already heard are more valuable than anything on the competitor's own website.
- **Re-run it when something changes** — a pricing update, a new feature launch, a funding round. Paste the new information into the same prompt structure rather than starting from scratch.
- **Never skip the fact-check step.** The instruction to flag gaps helps, but models can still be confidently wrong about specifics like exact pricing tiers — verify anything a rep will say as fact.
