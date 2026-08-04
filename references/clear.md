# CLEAR: strip the machine tells

Run this before the shift patterns. Tells are noise, and noise hides the real
problem. A sentence can pass every one of these and still leave the reader
smaller, which is what `references/edit.md` is for.

**Attribution.** This pass is a condensed distillation of the
[`humanizer`](https://github.com/blader/humanizer) skill by blader (MIT), which
is itself built on Wikipedia's *Signs of AI writing*. If you want the full
twenty nine pattern treatment with worked examples, install it alongside this
one and run it first:

```bash
git clone https://github.com/blader/humanizer.git ~/.claude/skills/humanizer
```

The two are complementary by design. `humanizer` clears the tells. `shift`
changes the standing. Running only the first leaves prose that is clean and
dead.

---

## Content

**C1. Inflated significance.** *stands as, serves as, is a testament to, plays a
vital role, underscores its importance, marking a pivotal moment, evolving
landscape, indelible mark.* Replace with the plain fact and its concrete
purpose.

**C2. Superficial analysis in participles.** Sentences with tails that begin
*highlighting, underscoring, emphasising, ensuring, reflecting, showcasing,
fostering, contributing to.* Delete the tail or replace it with an attributed
fact.

**C3. Promotional language.** *boasts, vibrant, rich, profound, groundbreaking,
renowned, breathtaking, must-visit, stunning, nestled, in the heart of.* State
what the thing is.

**C4. Vague attribution.** *industry reports, observers have cited, experts
argue, some critics say, several sources.* Name the source and the date, or drop
the claim.

**C5. Formulaic sections.** *Challenges and Future Prospects. Despite these
challenges. Future Outlook.* Replace with dated specifics.

## Language

**C6. The vocabulary.** *actually, additionally, align with, crucial, delve,
emphasising, enduring, enhance, fostering, garner, highlight, interplay,
intricate, key, landscape, pivotal, showcase, tapestry, testament, underscore,
valuable, vibrant.* They cluster. Finding one usually means finding four.

**C7. Copula avoidance.** *serves as, stands as, represents, boasts, features,
offers* where *is* or *has* would do.

**C8. Negative parallelism.** *Not only X but Y. It's not just about X, it's Y.*
Also clipped negative tails: *no guessing, no wasted motion.* State the point
directly.

**C9. Rule of three.** Three items where the material has two or five. Use the
number that is actually there.

**C10. Elegant variation.** Cycling synonyms for one thing (protagonist, main
character, central figure, hero) to avoid repeating a noun. Repeat the noun.

**C11. False ranges.** *from X to Y* where X and Y do not sit on a scale.

**C12. Passive voice and subjectless fragments.** *No configuration needed. The
results are preserved.* Name who does it.

## Style

**C13. Em dashes.** Machine prose uses them far more than people do, mimicking
punchy sales writing. Use commas, full stops, or parentheses.

**C14. Boldface scattered through prose** for mechanical emphasis.

**C15. Inline header lists.** `- **Performance:** Performance has been improved`
Convert to prose.

**C16. Title Case Headings.** Use sentence case.

**C17. Emoji** in headings and bullets.

**C18. Curly quotes** where straight ones belong in code or plain text.

## Communication

**C19. Assistant artifacts.** *I hope this helps, Certainly, Of course, You're
absolutely right, Would you like me to, let me know.*

**C20. Cutoff disclaimers.** *As of my last update, based on available
information, while specific details are limited.*

**C21. Sycophancy.** *Great question.* Answer the question.

## Filler

**C22. Padding.** *in order to* to. *due to the fact that* because. *at this
point in time* now. *in the event that* if. *has the ability to* can. *it is
important to note that* delete.

**C23. Stacked hedging.** *could potentially possibly be argued that it might
have some effect.* Say *may affect.*

**C24. Generic uplift endings.** *The future looks bright. Exciting times
ahead.* End on a fact or a plan.

**C25. Uniform hyphenation.** *third-party, cross-functional, client-facing,
data-driven, decision-making, real-time, end-to-end,* all hyphenated in one
document. People are less consistent than this.

**C26. Persuasive authority tropes.** *The real question is, at its core, in
reality, what really matters, fundamentally, the deeper issue.* These pretend to
cut through to a deeper truth, and the sentence that follows usually restates an
ordinary point with ceremony.

**C27. Signposting.** *Let's dive in, let's explore, let's break this down,
here's what you need to know, without further ado.* Announcing the thing instead
of doing it.

**C28. Fragmented headers.** A heading followed by one line restating the
heading.

**C29. Uniform sentence length.** Every sentence between twelve and eighteen
words. Vary the rhythm. Short ones land. Then let one run longer when the
thought actually needs the room to arrive somewhere.

---

## The pass

1. Read the text once, marking tells.
2. Fix them.
3. Ask yourself: *"What still makes this obviously machine written?"* Answer in
   bullets.
4. Fix those.
5. Hand the result to `references/edit.md`.

Clean is the floor here, not the ceiling. Everything interesting happens next.
