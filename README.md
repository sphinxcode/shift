# shift

A Claude Code skill for writing that leaves the reader more sovereign than it
found them.

Strip every em dash, every "delve", every rule of three, and you are left with
prose that is clean and dead. Clearing the machine tells is a real job and this
skill runs that pass first. Then it does the other thing, the one that actually
matters: it changes where the reader stands.

```bash
git clone https://github.com/sphinxcode/shift.git ~/.claude/skills/shift
```

## Two modes

**EDIT** rewrites a piece of text. Interface strings, onboarding, a landing
page, an error state, docs, an email.

**INHABIT** writes a voice instruction you paste into an assistant's system
prompt, so it speaks this way permanently. This is the part most writing skills
do not do.

There is also **CHECK**, which audits and reports without touching anything.
Useful in review.

## The three positions

| Position | What it does to the reader | Mechanism |
|---|---|---|
| Sovereignty | They own what is theirs | Authentic pride. Credit the act, never the trait |
| Regard | They are met without conditions | Unconditional positive regard. No evaluation attached |
| Expanse | Their frame widens | Awe. Vastness, plus something that will not fit the old frame |

## The distinction it turns on

Pride splits into two constructs that look identical on the page and do opposite
things to a person.

Authentic pride attributes an outcome to something specific they did. It tracks
with real self-esteem, persistence, generosity. Hubristic pride attributes it to
a fixed trait, and tracks with narcissism, low self-esteem underneath, and
brittleness. Praise someone for who they are and their next failure indicts
them, rather than the attempt.

Same split as person praise versus process praise. "You're so smart" produces
avoidance of hard tasks. "You found a good strategy" produces persistence.

Which means "own your gifts" is the wrong instruction, if a gift is something
you were given.

```diff
- You have a natural gift for reading people.
+ You noticed she went quiet, and you checked in later, privately.
```

Both affirm. Only the second gives someone something to stand on.

## Samples

### Interface copy

```diff
- Enter sends, Shift and Enter makes a line.
+ Send with Enter. Hold Shift if you're still writing.
```

The subject of the first sentence is a key. The reader is a spectator to their
own keyboard. The second also leaves a door open onto a real moment, instead of
closing the topic.

```diff
- A corner mark means Pro.
+ Open anything with a corner mark and look around. Pro brings the reading
+ with it.
```

"Means" asserts a static relation between two nouns and depicts no event.
Nothing happens, so nothing lands.

```diff
- Nine sections, forty-one pages, one button.
+ You're on one page of your chart. The switcher opens the rest.
```

A count hands someone a magnitude to measure themselves against. Enumeration
also lets a writer avoid having a view. List five and one of them might land.

```diff
- Just tap the icon, it's easy.
+ Tap the icon when you want it.
```

"Just" implies anyone competent finds this easy, so struggling means you are
not.

### Marketing

```diff
- Unlock your potential with our revolutionary personalized system! You have a
- natural gift for intuition, you just haven't tapped into it yet. Science
- confirms that when you begin within, everything shifts. Simply complete your
- profile. 70% OFF, next 30 minutes only.

+ Think of the last time you knew something before you could explain how.
+
+ That's the part of you this reads from. Give us your birth date, time and
+ place, and each morning you'll get one word drawn from it, with somewhere to
+ write down what it moved.
+
+ Birth time sharpens it. You can add that later if you have to go looking.
+
+ The annual plan is 70% less, and it'll be there when you want it.
```

Seven things changed. The trait claim went, because it builds the fragile kind
of pride. "You just haven't tapped into it yet" went, because that is a verdict
wearing encouragement. The unnamed appeal to science went, because a reader who
checks and finds nothing discounts everything else you said. The deadline went
and the price stayed, because the fact survives and the clock does not.

The opening is the load bearing change. It is a question rather than a claim,
which sends the reader to find their own evidence.

### An error state

```diff
- Invalid input. Please make sure you enter a valid email address.
+ That address didn't go through. Worth checking for a stray space at the end,
+ that catches most of them.
```

"Please make sure you" is a controlling construction with no rationale.

## Why the question matters more than the sentence

A sentence read passively will not durably move anyone. The evidence for single
line mood shifts is thin, mostly lab bound, and confounded by participants
guessing what the experimenter wants.

What holds up is stranger and much better. Brief exercises where a person spends
fifteen minutes writing about something they value have shown effects on
wellbeing and performance two to three years later, and in some groups longer.

The difference is who does the composing.

```diff
- Your strongest gift is listening.
+ Who talked to you this week when they wouldn't have talked to anyone else?
```

The first is a claim to accept or reject. The second sends them looking, and
what they find belongs to them.

So the order of preference is a question that makes the reader recall their own
evidence, then a concrete scene named precisely enough to be wrong, then a plain
statement with the reader as its subject, then anything else.

## What it detects

Sixteen patterns in three banks, each with trigger words, the mechanism, and a
before and after pair.

Content: trait praise where act praise belongs, contingent regard, diagnosis
without return, concepts wearing costumes, counting where naming belongs,
promised feeling.

Position: system as subject, controlling verbs, presupposed deficiency, copulas
and transactional verbs, missing stance, premature closure.

Commercial register: urgency and scarcity, benefit stacking, superlative and
comparison, borrowed authority.

Plus twenty nine machine tells in the CLEAR pass, condensed from
[`humanizer`](https://github.com/blader/humanizer).

## Working with humanizer

`humanizer` clears the tells. This changes the standing. They are complementary,
and running only the first leaves you with prose that is correct and inert.

`references/clear.md` carries a condensed version so the skill works standing
alone. For the full treatment with worked examples, install both and let this
one call it first.

```bash
git clone https://github.com/blader/humanizer.git ~/.claude/skills/humanizer
```

## Honesty about the grounding

The skill carries a full section on this, because a method that overstates its
basis gets dismissed by the people who would use it well.

**Established.** Authentic versus hubristic pride (Tracy and Robins, 2007).
Person versus process praise (Mueller and Dweck, 1998). Self determination
theory (Deci and Ryan). Autonomy supportive language as a coded, testable
distinction. Moral elevation (Haidt, 2000). Awe as vastness plus need for
accommodation (Keltner and Haidt, 2003). Unconditional positive regard. Values
affirmation writing with multi-year effects (Walton and Cohen).

**Contested.** Broaden and build's broadening mechanism. Durability of affect
shifts from short passive text. Second person address, which helps in affirming
contexts and can read as confrontational in corrective ones.

**Retracted, never cite.** The critical positivity ratio of 2.9013. The
modelling was formally withdrawn after Brown, Sokal and Friedman (2013) showed
the mathematics did not support it.

**Unsupported.** Vibration and frequency as literal descriptions of emotional
states. The idiom is New Thought by way of *The Secret*. Hawkins' Map of
Consciousness rests on applied kinesiology, which fails blinded testing.

Keep the word *vibration* if it is the honest name for what you are aiming at.
Do not attach *according to science* to it. The method does not need the claim,
and the claim is the part that gets the method dismissed.

One correction worth carrying: on Hawkins' own scale, Pride sits at 175 to 199,
below his 200 threshold, in the band he calls Force rather than Power. So
"divine pride", taken as a gesture toward that lineage, borrows the wrong rung
by that lineage's own reckoning. Authentic pride is a better foundation, and it
says something more useful. Pride is durable exactly when it is attached to what
a person did.

## Why it exists

Machine prose optimises for the most broadly applicable next token, so it
converges on statements that could be addressed to anyone. A sentence addressed
to anyone tells its reader they are no one in particular.

The repair is specificity aimed at one person, credit attached to what they
actually did, acceptance offered without a condition, and a door left open.

## Structure

```
shift/
  SKILL.md              the three positions, mode routing, grounding
  references/
    clear.md            29 machine tells, condensed from humanizer
    edit.md             16 patterns, the process, the counts, worked example
    inhabit.md          the voice template, filled example, handover notes
```

## Version history

**2.0.0** Two modes. INHABIT added, for setting an assistant's voice rather than
editing a document. CLEAR pass folded in from humanizer with attribution.
References split out of the single file.

**1.0.0** Three positions, sixteen patterns, two-pass audit, grounding section.

## License

MIT
