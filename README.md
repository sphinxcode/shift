# shift

A Claude Code skill that moves writing out of the commercial-instructional
register and into one that leaves the reader more sovereign than it found them.

Removing AI tells is a different job. Strip every em dash, every "delve," every
rule of three, and you are left with prose that is clean and dead. `shift` is
about something else: **where the reader stands after reading.**

```
/shift
```

Point it at copy — interface text, onboarding, notifications, landing pages,
error states, AI system prompts — and it rewrites for standing rather than
style.

## The three positions

| Position | What it does to the reader | Mechanism |
|---|---|---|
| **Sovereignty** | They own what is theirs | Authentic pride: credit the act, never the trait |
| **Regard** | They are met without conditions | Unconditional positive regard: no evaluation attached |
| **Expanse** | Their frame widens | Awe: vastness, plus something that will not fit the old frame |

## The distinction the whole thing turns on

Pride splits into two constructs that look identical on the page and do opposite
things to a reader.

**Authentic pride** attributes an outcome to something specific the person did.
It tracks with genuine self-esteem, persistence and generosity.

**Hubristic pride** attributes it to a fixed trait. It tracks with narcissism,
low self-esteem underneath, and brittleness — praise someone for who they are
and failure now indicts them rather than the attempt.

Same split as person-praise versus process-praise. "You're so smart" produces
avoidance of hard tasks; "you found a good strategy" produces persistence.

So:

> **Before:** You have a natural gift for reading people.
> **After:** You noticed she went quiet, and you checked in later, privately.

Both affirm. Only the second gives the reader something to stand on.

## Install

```bash
git clone https://github.com/sphinxcode/shift.git ~/.claude/skills/shift
```

Then `/shift` in Claude Code, or let it trigger on its description.

## What it detects

Sixteen patterns in four banks.

**Content** — trait praise where act praise belongs · contingent regard ·
diagnosis without return · concepts wearing costumes · counting where naming
belongs · promised feeling

**Position** — system as subject · controlling verbs · presupposed deficiency ·
copulas and transactional verbs · missing stance · premature closure

**Commercial register** — urgency and scarcity · benefit stacking · superlative
and comparison · borrowed authority

Each pattern ships with its trigger words, the mechanism, and a before/after
pair.

## The delivery principle

A sentence read passively will not durably move anyone. The evidence for
single-line mood shifts is thin and mostly lab-bound.

What holds up is stranger and better: brief exercises where a person spends
fifteen minutes writing about something they value have shown effects on
wellbeing and performance two to three years later.

**The difference is who does the composing.** So the highest form of this method
is not a better sentence — it is a sentence that invites the reader to say the
thing themselves.

> **Before:** Your strongest gift is listening.
> **After:** Who talked to you this week when they wouldn't have talked to
> anyone else?

The first is a claim to accept or reject. The second sends them to find the
evidence, and what they find is theirs.

## Honesty about the grounding

The skill carries a full section on this, because a method that overstates its
basis gets dismissed by exactly the people who would use it well.

- **Established** — authentic vs hubristic pride (Tracy & Robins 2007);
  person vs process praise (Mueller & Dweck 1998); self-determination theory
  (Deci & Ryan); autonomy-supportive language; moral elevation (Haidt 2000);
  awe as vastness plus accommodation (Keltner & Haidt 2003); unconditional
  positive regard; values-affirmation writing with multi-year effects
  (Walton & Cohen).
- **Contested** — broaden-and-build's broadening mechanism; durability of affect
  shifts from short passive text; second-person address in corrective framing.
- **Retracted, never cite** — the "critical positivity ratio" of 2.9013. The
  modelling was formally withdrawn after Brown, Sokal & Friedman (2013).
- **Unsupported** — "vibration" and "frequency" as literal descriptions of
  emotional states. The idiom is New Thought by way of *The Secret*. Hawkins'
  Map of Consciousness rests on applied kinesiology, which fails blinded
  testing.

Keep the word *vibration* if it is the honest name for what you are aiming at.
Do not attach *according to science* to it. The method does not need the claim,
and the claim is the part that gets the method dismissed.

## Why it exists

Machine prose optimises for the most broadly applicable next token, so it
converges on statements that could be addressed to anyone. A sentence addressed
to anyone tells its reader they are no one in particular.

The repair is specificity aimed at one person, credit attached to what they
actually did, acceptance offered without a condition, and a door left open.

## Version history

**1.0.0** — Initial release. Three positions, sixteen patterns, two-pass audit,
grounding section separating established from contested from unsupported.

## Related

- [`humanizer`](https://github.com/blader/humanizer) — removes AI writing
  patterns. Complementary: run `humanizer` to clear the tells, `shift` to change
  the standing. Clean and dead is still dead.

## License

MIT
