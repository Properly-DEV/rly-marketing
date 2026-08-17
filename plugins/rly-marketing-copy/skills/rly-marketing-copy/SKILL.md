---
name: rly-marketing-copy
description: Writes AND evaluates marketing copy for Properly (fintech/Web3 design studio) — website copy, blog articles, LinkedIn posts, and X posts/threads. Applies Properly's Voice & Format Guide, a storytelling craft toolkit, trend/topic packs, and a strict anti-AI-tells pass so nothing reads machine-written. Every generated draft comes with a scorecard (trend fit, persona fit, master-prompt compliance). Use this whenever anyone on the team wants to write, draft, rewrite, punch up, or shorten any Properly marketing/social/blog/website copy — even if they just say "write a post about X," "draft the branding page," "tweet this," or paste rough copy and ask to fix it. Also use it to score or review an existing draft — "score this post," "evaluate this draft," "is this on-brand," "which persona does this hit" — including posts written by other team members. English only.
user_invocable: true
---

# /rly-marketing-copy — Marketing copy for Properly

Write copy that sounds like a senior person who knows finance and design cold, and that no reader could mistake for AI. One voice lives here: **Properly**, the company voice. This file routes you to the right context and runs the guardrail. All output is English.

The reference files carry the real substance. This file is the map and the workflow. Don't skip the reads — the rules reference each other, and the parts that get skipped are the ones that keep copy from going generic.

## The files

- `references/properly-voice-guide.md` — **the frozen source of truth.** The full Voice & Format Guide, verbatim. It owns Properly's voice, the Five Rules, the banned words, the per-channel format/length specs (§3), the keywords (§4), the ICP personas (§6), and the **only approved list of client numbers and proof points (§5)**. Never edit it.
- `references/storytelling-toolkit.md` — the craft: hooks, PAS/BAB/StoryBrand, narrative arc, show-don't-tell, the "so what?" ladder, open loops, rhythm.
- `references/company-showcase.md` — **the Properly company-post shape** (thesis → deepen → solution → visualization), grounded in a real project and closing on the solution. Read it for any substantive company post; it's what separates a showcase from a "website for XYZ" caption.
- `references/anti-ai-tells.md` — the anti-AI layer: extended banned words, structural/formatting/tonal/rhythm tells, and the pre-ship checklist. Run this every time.
- `examples/properly-examples.md` — Properly's canonical specimens plus before/after pairs.
- `topics/_index.md` — registry of theme packs (ETF, RWA, stablecoins, regulated crypto, fraud, agentic finance, and more). Each pack carries SEO keywords, trending angles, ready-made narrative theses, and the §5 clients that anchor the theme. Read the index to pick the right pack when a post has a clear subject.
- `references/scorecard.md` — the evaluation rubric: scores any draft 1–5 on trend fit, persona fit, and master-prompt compliance, with a verdict and ranked fixes. Used to append a scorecard to every generated draft, and to review a pasted draft on its own.

## Workflow

Two modes. **Write mode** (the default): follow steps 1–7. **Evaluate mode**: someone pastes a finished post (their own, a teammate's, an old draft) and wants it judged, not rewritten — cues like "score this post," "is this on-brand," "which persona does this hit," "review this draft." In evaluate mode, skip the writing (step 4) and go straight to step 7, scoring the pasted text as-is. Detect channel and topic first (step 1) so you score against the right rules; the core-message confirmation in step 1 applies to write mode only. Every write-mode result is assembled in the fixed **Output order** below.

## Output order — always, every destination

Every write-mode result ships as one block in this exact order, whether it lands in an Obsidian note, a Claude artifact, a chat reply, or anywhere else. Same order every time, so anyone opening a Properly draft knows where to look. Never reorder these:

1. **Overview** — the narrative/thesis in one line, the topic pack in play, the ICP/persona, and the core message. Any working notes or sources live here, at the top.
2. **LinkedIn** — the post.
3. **X** — the post or thread.
4. **Next posts** — three follow-up ideas on the same topic, one sentence each (step 6).
5. **Scorecard** — always the final block (step 7).

If the user asks for several versions of one topic at once, each full draft repeats this same order.

### 1. Detect the channel, the topic, and the core message

**Channel.** Website, blog, LinkedIn, or X. Name it explicitly, because these are different registers, not long and short versions of one thing. A LinkedIn post and a tweet are written differently here. If the brief doesn't say, ask one line.

**Topic.** If the post has a clear subject (a client, a trend, a service theme), check `topics/_index.md` and match it to a theme pack via that file's `match:` triggers, which include client names. Load at most one or two packs. A theme pack gives you SEO keywords, a dated trend to hook on, ready-made narrative theses, and the §5 clients that anchor the theme. If nothing matches, write without a theme layer or ask one line which theme fits. Read the top of `topics/_index.md` first — it sets the keyword-weaving and numbers discipline for every pack.

**Project.** A company showcase post is grounded in a specific client project. The brief names the project and its background up front — use that for the deepen and solution beats. Never assume a project or reuse one from a past post; if it's missing for a showcase post, ask which project and for its context. Whether the name appears in the published copy follows §5 (see `company-showcase.md`) — NDAX is just one example of a nameable client, not a default.

**Message. Confirm the one thing the post is there to say before writing a line.** Writing from a bare topic is the fastest route to a competent post that could've been written by anyone, which is exactly the shallowness to avoid. So always lock the core message first, and adapt how you get it:

- **A clear point of view, or a rich brain dump, is already in the brief** → don't ask from a blank page. Restate the core message you've extracted in one line and confirm it: *"The main point I'm taking is X — writing on that?"* Write once it's confirmed or corrected. This one-line check is quick and catches the times you'd have run with the wrong angle.
- **The brief is thin (a topic and nothing more)** → ask straight out: *"What's the one thing you want the reader to take away — your angle on this?"* If the author isn't sure, offer 2–3 candidate theses from the matched topic pack as a starting point, always ending with "or something else," so they're prompted, not railroaded into a generic pack line.
- **They say "you decide"** → pick a pack thesis, write, and name the angle you chose in the scorecard so the choice is visible, not buried.

Keep it to one line, ask at most once, don't stall the work. This step is where the depth you actually want gets in; skipping it is what flattens the copy.

### 2. Load the right context

- Read `properly-voice-guide.md` in full. It's short and every section earns its place. Glance at `examples/properly-examples.md` — the voice transfers by imitation faster than by rule.
- **If a topic matched** → read the matched `topics/*.md` pack. Weave 1–2 primary keywords naturally (blog/web only; on social, use the theme to pick a timely subject and the reader's vocabulary, not to cram phrases). Reach for one narrative thesis and write it in the voice. Anchor with the pack's §5 clients, never its external companies.
- **Always** → pull `storytelling-toolkit.md` for the craft and keep `anti-ai-tells.md` open for the guardrail.

### 3. The numbers rule (hard)

Every metric, client outcome, percentage, and named proof point about **Properly's work** must exist in the guide's **§5**. If the specific figure you want isn't there, write around it or reach for a different true detail. **Never invent or estimate a number.** This is the guide's most load-bearing rule and the fastest way to embarrass the studio.

Topic packs contain **external market-context figures** (industry AUM, market-size projections, a competitor's headcount). Those are a different category: dated third-party context, useful to establish a trend, never a Properly result. Keep them clearly external, verify a hard number before it ships, and never blend a market stat with a Properly claim in the same breath.

### 4. Write

Only start once the core message from step 1 is locked. Build the whole piece to land that one point. Open on a real hook (a specific, a position, a moment — never a throat-clear). Pick a structure from the toolkit that fits the piece; a short post might lean on one technique, a blog article on several. Enter the conversation already in the reader's head. Show, don't tell. Vary sentence length hard. Hold to the channel's length spec in §3. Keep the reader ("your") as the subject more than the studio ("we").

For a **Properly company post**, default to the showcase shape in `company-showcase.md`: thesis → deepen (grounded in **the project named in the brief** — the user states it and its background up front) → solution → visualization. **Close on the solution, not a question** — the company account exists to hand the reader something real, not to leave a thought hanging.

### 5. Pre-ship anti-AI pass (the gate)

Before showing anything, run the checklist at the bottom of `anti-ai-tells.md`. The three that catch the most, every time:

1. **Negative comparison** — no "not X but Y," "it's not about X, it's Y," "doesn't just X, it Y," no stacked contrasts. Rewrite as a positive statement of what the thing IS. This is the number-one tell. (Guide §2 allows exactly one exception: a single reversal as a closing line, both halves factually true.)
2. **Banned words** — check the guide's §2 list *and* the extended list in `anti-ai-tells.md`. Replace with the specific thing or cut.
3. **Length vs channel** — measure against §3 for this exact channel. LinkedIn and X are counted in **characters, not words** (finance words run long, so a word count reads short). Check the character band, and on LinkedIn watch the paragraph count too: 6+ blocks reads long even inside the limit.

Then the rest: numbers trace to §5, rhythm isn't a metronome, no over-bolding or emoji-bullets or title-case headers, and the say-it-out-loud test passes. Fix before presenting, don't present with caveats.

### 6. Propose three next angles

After the post, always propose three follow-up posts: the same topic, a different angle each, one sentence apiece. Social feeds forget fast, so a fresh take on the same subject lands again a couple of weeks later without reading as a repeat. Pull the angles from the topic pack's other theses and from different hooks and frameworks in `storytelling-toolkit.md`, so each is a genuinely different take rather than the same post reworded. Use this shape:

```
Next posts (same topic, different angles):
1. <angle> — <one sentence on the take>
2. <angle> — <one sentence>
3. <angle> — <one sentence>
```

If the user wants, write any or all of them as full drafts, each following the same Output order. One topic or one brain dump then becomes several ready posts to pick the best from or bank for later. When they brief a topic and ask up front for "a few versions" or "all the angles," skip straight to writing the set — one full draft per angle, each with its own scorecard.

### 7. Score the draft (always, the last block)

Run `references/scorecard.md` and place the scorecard as the **final block**, after the three proposals. This is not optional — every generated draft ships with its self-assessment on the three dimensions (trend fit, persona fit, master-prompt compliance), a verdict, and ranked fixes. Score honestly; an all-5s scorecard is a red flag, not a win.

If this draft is a revision of one already scored this session, show the per-dimension delta (was N ▲/▼) so the improvement is visible. In evaluate mode, the scorecard *is* the deliverable — lead with it, and you can still offer three next angles after it.

## When handing back

Give the copy clean and ready to paste. If the brief asked for a channel with mechanics (LinkedIn link-in-first-comment, X thread structure), note those briefly after the copy. If you had to write around a missing number, say so in one line so the author can drop in the real figure.
