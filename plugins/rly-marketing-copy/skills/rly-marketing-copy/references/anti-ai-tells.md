# The Anti-AI Layer

This is the guardrail that keeps output from reading as machine-written. The guide's §2 already bans the highest-value offenders (negative comparison, its banned-words list, em-dashes). This file extends that with everything else a reader now uses to spot generated text.

**The one principle that matters most:** no single item here is proof on its own. Real writers use some of these words sometimes. What gives AI away is **density** — three or more tells clustered in a short stretch. An editor flags text when the pile-up appears, not when one "utilize" shows up. So the goal isn't zero instances of any one word. It's writing that never clusters, never falls into the safe rhythm, always reaches for the specific. Aim near-zero and you'll land in the human range.

Read this before drafting so you avoid the tells on the way out, and run the checklist at the bottom before showing the copy to anyone.

---

## 1. Words and phrases to cut

These stack on top of the guide's banned list, they don't replace it. When you catch one, don't swap in a synonym — usually the fix is to name the actual thing or delete the word.

**Prestige-abstraction nouns** (borrowed grandeur bolted onto ordinary things):
tapestry · landscape · realm · mosaic · symphony · labyrinth · beacon · cornerstone · bedrock · testament · treasure trove · odyssey · sentinel · interplay · fabric (figurative) · lens (figurative "through the lens of")
→ Name the literal thing. Not "the fintech landscape," just "fintech." Not "a testament to the team's work," just say what the team did.

**Inflated Latinate verbs** (on top of the guide's leverage/empower/elevate):
utilize · harness · facilitate · optimize · navigate · illuminate · bolster · foster · unlock · unleash · embark · delve · dive (into) · garner · underscore · underpin · showcase · spearhead · revolutionize · redefine · democratize · cultivate · encompass · exemplify · streamline · commence · endeavor
→ Use the short Anglo-Saxon word. "Use" not "utilize." "Start" not "commence." "Help" not "facilitate." "Show" not "showcase." The shortest correct verb wins.

**Corporate/dramatic adjectives** (on top of world-class/seamless/cutting-edge):
robust · vibrant · dynamic · comprehensive · multifaceted · nuanced · holistic · groundbreaking · unparalleled · meticulous · intricate · pivotal · crucial · vital · profound · remarkable · noteworthy · rich (figurative) · diverse array of
→ Be specific or delete it. "Robust system" → "handles 10k requests a second." Most of these can simply be cut with no loss.

**Signposting adverbs and hedges** (these run at several times the human rate):
moreover · furthermore · additionally · notably · arguably · importantly · significantly · essentially · ultimately · indeed · crucially · that said · potentially
→ Most transitions can just be deleted. If you truly need one, "and," "but," "so," "also" read human.

**Travel-brochure register:**
nestled · boasts · brimming with · steeped in · breathtaking · stunning · picturesque · renowned · iconic · in the heart of · hidden gem
→ A concrete detail beats the adjective every time.

**Phrase templates — the sentence-level tics:**
- "It's important to note that…" / "It's worth noting…"
- "In today's fast-paced world…" / "In the fast-paced world of…"
- "When it comes to…"
- "At its core…" / "At the end of the day…"
- "Navigating the complexities of…" / "Navigating the landscape of…"
- "Plays a vital/pivotal/crucial role in…"
- "Stands as a testament to…" / "Serves as a reminder that…"
- "From X to Y" as filler enumeration ("from onboarding to retention")
- "Whether you're a X or a Y…"
- "Let's dive in" / "Let's unpack this" / "Let's explore"
- "In the world of…" / "In the realm of…"

## 2. Structural and rhetorical tells

- **Copula avoidance.** AI won't write "is." It reaches for "serves as," "stands as," "represents," "functions as," "boasts," "features." → Just write "is." Plain copulas are human.
- **The five-paragraph-essay reflex.** Intro, three balanced body chunks, a recap, applied even to a 100-word post. → Start in the middle. End when the point is made. Cut the recap.
- **Both-sides hedging.** Presenting a balanced view even when one side is obviously right, then landing on "both have their merits." This is the opposite of the guide's Rule 3. → Take a position. Say which one you'd pick and why.
- **The "challenges and future" wrap.** "Despite its promise, [thing] faces several challenges… only time will tell." → Leave things unresolved without announcing that you're doing it. An honest "we don't know yet how this plays out" does this right; the formulaic version does it wrong.
- **Fake lists.** "Here are five ways to…" where it's one idea restated five times. → If you have two real points, write two.
- **Symmetrical list items.** Every bullet the same length and shape. Real lists are lumpy. → Let items be uneven: one a full sentence, the next three words.
- **Participial-phrase openers.** "Boasting a clean interface…", "Offering a range of…", "Ensuring that…", "Reflecting a broader trend…". The "-ing opener" runs several times the human rate. → Start with the subject. "The tool offers X," not "Offering X, the tool…"
- **The floating participial tail.** A clause tacked on to restate what you just said: "…marking a pivotal moment for the industry." → Delete the tail. It adds nothing.
- **Ghost citations.** "Studies show…", "Experts agree…", "Research suggests…" with nobody named. → Name the source or drop the claim. (For Properly, numbers come from §5 only.)
- **Over-explaining the obvious.** Defining KYC to an audience of fintech founders. → Trust the reader. The guide's Rule 1 says the same.
- **Personifying abstractions.** "The data tells a story," "the market spoke." → People act, concepts don't.

## 3. Formatting tells

- **Over-bolding.** Mechanically bolding key terms across a paragraph. → Bold almost nothing. (The guide's blog spec allows bolding a key term *once* when it's introduced. That's the ceiling.)
- **Emoji bullets or section markers** (🚀 🔑 💡 ✅). A dead giveaway. → Plain text. The guide allows at most one emoji, at the very end of a LinkedIn post.
- **Title Case Headers.** "The Impact Of Design On Trust." → Sentence case.
- **Colon-headlines.** "Trust: Why Design Matters in Finance." → Rewrite as a plain phrase.
- **"In conclusion / In summary / Ultimately" wrap-ups.** → End on your last real point.
- **Zero contractions.** "cannot," "do not," "it is." → "can't," "don't," "it's." The guide mandates contractions everywhere, including the website.
- **Prose chopped into nested bullets** when it's an argument, not an inventory. → Write paragraphs when you're making a case. Properly's posts are almost all prose for this reason.

## 4. Tonal tells

- **Motivational-poster positivity.** Everything's an "opportunity," no tension, no downside, nothing ever sucks. → Admit what's hard. Name a real risk. The guide's honesty ("this won't work," "we don't") does this.
- **Sycophancy.** "Great question!" "What a fantastic point!" → Just say the thing.
- **Tonal sprinkles.** "Hope this helps!" "Let me know if you'd like me to expand!" → Stop when the content stops.
- **False profundity.** Ending a paragraph on a fortune-cookie line: "Because in the end, design is about people." → End on a fact or a specific, not an aphorism.
- **Manufactured energy.** "Let's dive in!" at the top. → Open cold, mid-thought.
- **Inflated significance.** Calling a minor thing "transformative" or "a game-changer." → Keep proportion. Small things are small.

## 5. Rhythm and grammar tells

- **Uniform sentence length.** The biggest structural tell. AI clusters everything around 15–20 words. → Swing hard. A four-word sentence next to a thirty-word one. See the rhythm section of the storytelling toolkit.
- **Elegant variation.** Compulsively swapping synonyms to avoid repeating a word. → Repeat the word. Repetition is human and clear.
- **Adverb padding.** "carefully," "seamlessly," "effortlessly," "meticulously." The "polish this" instinct adds modifiers. → Cut the -ly words. Let the verb carry it.
- **Present-participle overload.** Sentences stuffed with "-ing" clauses ("ensuring," "enabling," "allowing," "highlighting"). → Convert to plain finite verbs.
- **Everything grammatically perfect and safe.** No fragments, no sentence starting with "And," nothing that surprises. → Break a rule on purpose. Use a fragment. Trail off. Pick the less obvious word occasionally.

---

## Pre-ship checklist

Run this on every draft before showing it. The first three are the guide's own top-three failure points, promoted here because they catch the most.

1. **Negative comparison** — scan for "not X but Y," "it's not about X, it's Y," "doesn't just X, it Y," and back-to-back contrasts. This is the number-one tell. Rewrite as a positive statement of what the thing IS. The guide's §2 now allows one exception: a single reversal used as a closing line, where both halves are factually true. Anywhere else in the text, or stacked, it's still the tell.
2. **Banned words** — check against the guide's §2 list *and* section 1 above. Any hit gets cut or replaced with the specific thing.
3. **Length vs channel** — measure against the guide's §3 spec for this exact channel.
4. **Numbers are real** — every figure traces to §5 of the guide. No exceptions.
5. **Rhythm** — read it aloud. If it's a metronome, break the pattern. At least one short sentence next to a long one.
6. **Density scan** — read any 150-word stretch. If three or more tells from this file cluster there, that passage is the weak point. Fix it before anything else.
7. **Opening** — is the first line a real hook (a specific, a position, a moment), or a throat-clear? If it could open a competitor's post unchanged, rewrite it.
8. **The say-it-out-loud test** — would a senior person actually say this to a peer? If it sounds like a brand or a bot, it's not done.
