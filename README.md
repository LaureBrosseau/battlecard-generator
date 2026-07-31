# Battlecard Generator

Leverage this framework and AI prompts to turn raw competitive data into a sales-ready battlecard in a few minutes.

## Why battlecards matter

Sometimes sales reps lose deals to competitors because they didn't know how to respond or what to say when the competitor's name or arguments came up in a conversation with a prospect.
Battlecards help close that gap: they turn competitive intelligence that usually exists somewhere, in a Product Marketing Manager's head, in a sales rep's memory of a tough prospect call, in an old Slack thread.. but rarely anywhere a sales rep can actually access it live. 

## The problem

But many competitive battlecards are ineffective for the same reasons:  
- They're built once and barely updated, so sales stop using them.
- They're too long, too exhaustive, thus not usable in real-life situations.
- They often tell sales reps *what* the competitor does, but not *what to say* or *how to answer* against specific arguments.

A good battlecard is short, usable, straight to the point. It helps the sales rep quickly understand the ins and outs of a specific competitor.  

So here's what you'll find in this repo: a repeatable structure, a ready-to-use prompt, and battlecard examples, so anyone in Product Marketing can go from scattered competitor notes to a usable battlecard fast, with or without AI.

## What's in this repo

| File | What it's for |
|---|---|
| [`framework.md`](./framework.md) | The battlecard structure itself, the 9 sections every battlecard should have, and why |
| [`prompt.md`](./prompt.md) | Two ready-to-use prompts for Claude/ChatGPT: 1st one turns raw research (pricing pages, reviews, call notes) into a battlecard following my framework, 2nd one formats the battlecard into a HTML template. |
| [`example-filled.md`](./example-filled.md) | Lower/mid-market example (Flowbase vs. Taskly) |
| [`example-filled-enterprise.md`](./example-filled-enterprise.md) | Enterprise example (Structura vs. Vertex) |
| [`battlecard-template.html`](./battlecard-template.html) | A printable one-pager format sales can keep open during a call — pre-filled with the Flowbase/Taskly example, ready to duplicate and adapt with your own content. Can also be imported into Canva for further editing (see prompt.md). |

## How to use it

1. Gather raw data on your competitor: pricing page, G2/Capterra reviews, recent changelog or launch announcements, call notes where reps mentioned them, LinkedIn posts from their leadership..
2. Paste that raw material into the prompt in [`prompt.md`](./prompt.md), along with your own product's positioning.
3. Review and correct the AI output, never ship a battlecard you haven't fact-checked. AI helps accelerate the battlecard creation but you should always verify data before sharing it with sales reps.  
4. Once finalized, run it by a sales rep who knows well this specific competitor, they'll help validate the content and tell you if they'd phrase something differently on a call. If so, ask why, and revise your battlecard based on their answer.
5. Set a recurring reminder (monthly, or triggered by a competitor product update) to refresh it, an outdated battlecard is worse than no battlecard.

## Why this approach

At Akeneo, I owned competitive intelligence for all our offers. Sales reps need concrete arguments, not marketing fluff, to have conversations with the prospects about the competition. The framework reflects what sales actually need, not what looks good in a slide deck.

## About me

I'm Laure, a Product Marketing and Strategic Projects leader exploring how AI can make Product Marketing Managers work faster while keeping the quality bar high.  
More at [laurebrosseau.com](https://laurebrosseau.com). [Connect on LinkedIn](https://www.linkedin.com/in/laurebrosseau/).
