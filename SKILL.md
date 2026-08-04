---
name: shift
version: 2.0.0
description: |
  Shift writing into a register that leaves the reader more sovereign than it
  found them. Two modes. EDIT rewrites existing copy (interface text,
  onboarding, landing pages, error states, docs). INHABIT emits a voice
  instruction you paste into an AI so it speaks this way permanently. Runs a
  CLEAR pass first to strip AI tells, because clean and dead is still dead.
  Use when text is technically correct but reads as robotic, transactional,
  salesy, or subtly diminishing, or when an assistant's voice needs setting.
  Detects and repairs: trait praise, contingent regard, controlling verbs,
  urgency and scarcity, benefit stacking, system-as-subject, counting instead
  of naming, concepts wearing costumes, premature closure, missing stance.
license: MIT
compatibility: claude-code opencode
allowed-tools:
  - Read
  - Write
  - Edit
  - Grep
  - Glob
  - AskUserQuestion
---

# Shift: raise the standing of the reader

Removing the machine tells from a piece of writing leaves you with prose that is
clean and dead. That is a different job from this one.

This skill works on **where the reader stands after reading.**

## The three positions

Everything here comes from these.

| Position | What it does to the reader | The mechanism underneath |
|---|---|---|
| **Sovereignty** | They own what is theirs | Authentic pride. Credit the act, never the trait |
| **Regard** | They are met without conditions | Unconditional positive regard. No evaluation attached |
| **Expanse** | Their frame widens | Awe. Vastness, plus something that will not fit the old frame |

## The distinction the method turns on

Pride splits into two constructs that look identical on the page and do opposite
things to a person.

**Authentic pride** attributes an outcome to something specific they did. It
tracks with genuine self-esteem, persistence, generosity.

**Hubristic pride** attributes it to a fixed trait. It tracks with narcissism,
low self-esteem underneath, and brittleness. Praise someone for who they are and
their next failure indicts them rather than the attempt.

This is the same split as person praise versus process praise. "You're so smart"
produces avoidance of hard tasks. "You found a good strategy" produces
persistence.

So **"own your gifts" is the wrong instruction** if a gift is something you were
given.

> **Before:** You have a natural gift for reading people.
> **After:** You noticed she went quiet, and you checked in later, privately.

Both affirm. Only the second gives the reader something to stand on.

---

## Pick a mode

Ask which one applies. If the request is ambiguous, use `AskUserQuestion`.

### EDIT: rewrite a piece of text

The user has copy that needs shifting. Interface strings, onboarding, a landing
page, an error state, documentation, an email.

1. Read `references/clear.md`. Run the CLEAR pass first. Machine tells are noise
   that hides the real problem.
2. Read `references/edit.md`. Run the sixteen patterns, the two-pass audit, and
   the counts.
3. Return the four artifacts named in `references/edit.md`.

### INHABIT: set an AI's voice

The user wants an assistant to speak this way permanently, not to have one piece
rewritten. They will paste the result into a system prompt.

1. Read `references/inhabit.md`.
2. Ask what you need: what the assistant is for, who it speaks to, what it must
   never claim, whether it has domain jargon to handle.
3. Emit the voice block, filled in for their case.

Do not emit a generic block. An unfilled voice instruction produces the same
averaged prose this skill exists to repair.

### CHECK: audit without rewriting

The user wants to know what is wrong, not to have it fixed. Useful in review.

Run the counts from `references/edit.md` and report each failure with its line,
its pattern number, and which position it costs. Change nothing.

---

## The delivery principle

This governs both modes, so it lives here rather than in a reference.

A sentence read passively will not durably move anyone. Evidence for single line
mood shifts is thin, mostly lab bound, and confounded by participants guessing
what the experimenter wants.

What does hold up is stranger. Brief exercises where a person spends fifteen
minutes writing about something they value have produced effects on wellbeing
and performance two to three years later, and in some groups longer.

**The difference is who does the composing.** The durable version is self
generated, at an apt moment, in a context that supports it. It changes how the
reader interprets their own later experience.

So the highest form of this method is not a better sentence. It is a sentence
that invites the reader to say the thing themselves.

> **Before:** Your strongest gift is listening.
> **After:** Who talked to you this week when they wouldn't have talked to
> anyone else?

The first is a claim to accept or reject. The second sends them to find the
evidence, and what they find is theirs.

Prefer, in this order:

1. A question that makes the reader recall their own specific evidence.
2. A concrete scene from their life, named precisely enough to be wrong.
3. A plain statement of fact with the reader as its subject.
4. Anything else.

---

## What this is grounded in

Read this before defending the method to anyone. Overstating the basis is how a
good method gets dismissed.

**Established.** Authentic versus hubristic pride as distinct constructs with
opposite correlates (Tracy and Robins, 2007). Person praise versus process
praise producing fixed versus growth mindsets (Mueller and Dweck, 1998; Kamins
and Dweck, 1999). Self determination theory's three needs, autonomy, competence
and relatedness (Deci and Ryan), among the most replicated frameworks in
motivational psychology. Autonomy supportive versus controlling language as a
coded, testable distinction. Moral elevation as a distinct emotion with
prosocial downstream effects (Haidt, 2000; Pohling and Diessner meta analysis,
2016). Awe as vastness plus need for accommodation (Keltner and Haidt, 2003),
with its documented shift toward wider self categories (Shiota, Keltner and
Mossman, 2007). Unconditional positive regard, with modest but real effect
sizes. Brief self generated values affirmation writing producing effects years
later (Walton and Cohen; Cohen et al.).

**Contested.** Broaden and build's broadening mechanism specifically. The
durability of any affect shift from short passive text. Second person address,
which helps in affirming contexts and can read as confrontational in corrective
ones.

**Retracted. Never cite it.** The critical positivity ratio of 2.9013
(Fredrickson and Losada, 2005). The modelling and the numbers were formally
withdrawn after Brown, Sokal and Friedman (2013) showed the mathematics did not
support them. Use no numeric ratio of positive to negative. The directional
claim survives. The arithmetic does not.

**Unsupported.** Vibration and frequency as literal descriptions of emotional
states. The idiom comes from New Thought, specifically Atkinson's *Thought
Vibration* (1906), by way of *The Secret*, with a later coat of borrowed quantum
vocabulary. David Hawkins' Map of Consciousness, which assigns numeric
calibrations to emotions, rests on applied kinesiology. Blinded tests find
testers cannot distinguish true from false statements once they do not already
know the answer. No published raw data, no falsification path.

Keep the word *vibration* if it is the honest name for what you are aiming at.
Do not attach *according to science* to it. The method does not need the claim,
and the claim is the part that gets the method dismissed.

**One correction worth carrying.** On Hawkins' own scale, Pride sits at 175 to
199, below his 200 threshold, in the band he calls Force rather than Power. He
treats it as brittle and prone to collapsing into shame. So "divine pride,"
taken as a gesture toward that lineage, borrows the wrong rung by that lineage's
own reckoning. The psychology of authentic pride is a better foundation and says
something more useful: pride is durable exactly when it is attached to what a
person did.

---

## Why this exists

Machine prose optimises for the most broadly applicable next token, so it
converges on statements that could be addressed to anyone. A sentence addressed
to anyone tells its reader they are no one in particular.

The repair is specificity aimed at one person, credit attached to what they
actually did, acceptance offered without a condition, and a door left open.
