# The Scorecard

Every draft gets scored on three dimensions before it's handed over: **Trend fit**, **Persona fit**, **Master-prompt compliance**. This isn't decoration. It turns the silent pre-ship gate into a visible, honest assessment that points at exact rules, so the next iteration is a fix, not a reshuffle.

Two situations, one rubric:
- **Generate-then-score** — after writing a draft (including from a brain dump), append the scorecard beneath it automatically. It's the self-assessment on the work you just did.
- **Evaluate-only** — someone pastes a finished post (an employee's own draft, or an old one) and wants it judged. Skip writing; produce the scorecard against the pasted text.

When a draft is a revision of one you already scored, re-score and show the **delta** per dimension (see the bottom).

## The one rule for the scorer itself

Be a critic, not a cheerleader. Inflated praise is its own AI tell, and a scorecard that says 5/5 on everything is useless. If something is a 3, call it a 3 and say why. The value is in the honest weakness and the specific fix, not the number.

## The 1–5 scale

- **5** — exemplary on this dimension, ship as-is.
- **4** — strong, one minor tweak at most.
- **3** — acceptable but has a real weakness worth fixing.
- **2** — misses on this dimension, needs rework.
- **1** — fails or points the wrong way.

## Dimension 1 — Trend fit (does the subject ride a live trend?)

Score against `topics/`:
- **Which pack does the subject match** (via `_index.md`)? A clear match with the pack's angle is the baseline for a 4+.
- **Is the angle timely?** It should hook on a current, dated trend from the pack, not an evergreen truism. A post that could've run three years ago scores lower.
- **Keywords** (blog/web only): are 1–2 primary keywords woven in naturally? Missing them caps a blog/web post at 3; *stuffed* keywords are worse — that's a Master-prompt hit, not a trend win.
- **Narrative thesis:** did it use one of the pack's theses well, or invent a weaker angle?

A subject that fits **no** pack isn't automatically low — a deliberate evergreen or a client-story post can be a 4. But flag it: "no topic pack matched; is this intentional?"

## Dimension 2 — Persona fit (is it written for the right reader?)

Score against the guide's §6 ICP cheat sheet (Operator / Builder / Founder, 40/40/20):
- **Name the primary persona** the draft targets. A post should have one clear reader, not address all three at once.
- **Does it follow that persona's "Say"** and avoid its "Don't say"? Examples: an Operator post that opens with process (not outcome) misses; a Builder post that leads with aesthetic vision before a product observation misses; a Founder post with a discovery-questionnaire tone misses.
- **Right reader for the channel?** A CMO-facing brand argument reads differently on X than on the website.
- Judge whether the post speaks to a real, specific reader, not a generic "audience."

If the draft targets no identifiable persona, that's a 2: it's talking to everyone and landing with no one.

## Dimension 3 — Master-prompt compliance (does it obey the guide + anti-AI layer?)

This runs the pre-ship checklist from `anti-ai-tells.md` and the guide, and scores the result. Check, in priority order:
1. **Negative comparison** (§2) — the number-one tell. Any "not X but Y" / "doesn't just X, it Y" / stacked contrasts.
2. **Banned words** (§2 + `anti-ai-tells.md` §1).
3. **Numbers** — every Properly figure traces to §5; market stats stay flagged as external context.
4. **Length vs channel** (§3) — LinkedIn/X in characters, not words; watch paragraph count.
5. **Anti-AI density** — no cluster of tells in any 150-word stretch; rhythm varies; opening is a real hook.
6. **House style** — contractions, no em-dashes in the copy, capitalisation (Web3/DeFi/KYC).

**Hard caps** (a violation here caps this dimension regardless of the rest):
- An invented number (not in §5, or a market stat dressed as a Properly result) → **cap at 2**.
- Stacked negative comparisons, or a banned word left in → **cap at 3**.
- Over the channel's length ceiling → **cap at 3**.

## Output format

Append exactly this block (plain text, no emoji bullets), filled in:

```
── SCORECARD ──────────────────────────────
Voice: Properly · Channel: <…> · Topic: <pack or "none">

1. Trend fit          N/5   <one-line finding>
2. Persona fit        N/5   <primary persona + one-line finding>
3. Master-prompt      N/5   <one-line finding, cite § where relevant>

Verdict: <SHIP | REVISE | REWORK>
Top fixes:
  1. <fix, pointing at a rule/§>
  2. <fix>
  3. <fix>
───────────────────────────────────────────
```

Rules for the block:
- **Verdict thresholds:** SHIP = all three ≥4 and no hard cap triggered. REVISE = fixable in one pass (dims mostly 3–4). REWORK = any dimension ≤2, or a hard cap triggered.
- **Top fixes:** ranked by impact, each tied to a rule or § so the feedback is actionable ("§2 — negative comparison in para 3"), never vague ("make it punchier"). If the verdict is SHIP, write "none — ready" instead of padding three fixes.
- Keep findings to one line each. The detail lives in the fixes.

## Iterations — showing the delta

When re-scoring a revised draft, add the previous score in parentheses and an arrow, so progress is visible:

```
1. Trend fit          4/5 (was 3 ▲)   <what changed>
2. Persona fit        4/5 (was 3 ▲)   …
3. Master-prompt      5/5 (was 4 ▲)   …
```

If a dimension dropped, show it (`▼`) and say why — sometimes a fix for one rule breaks another (e.g. cutting length hurt the hook). The goal across iterations is every dimension at 4–5 with a SHIP verdict, reached by real fixes, not by relaxing the rubric.
