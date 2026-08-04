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

## The three tests

Ask them in order. Most bad sentences die at the first.

**1. Should this sentence exist?** Cut before you rewrite. Anything the reader
already knows, anything the interface already says, anything true of every
product, any courtesy padding after a complete thought. No rewrite saves a
sentence that should not be there.

**2. Where does it leave them?** Larger, level, or smaller. Level is the failure
state, not the safe state, and it is where careful writers land most often.
Clearer information is still level. Ask what the reader has that they did not
have before. If the answer is "the information in the sentence", it is level.

**3. Would a person say this out loud?** Read it. If you would not say it to
someone across a table, cut it. Straining for lyric produces sentences nobody
says, and it feels like craft while you are doing it.

## Samples

### Trait to act

```diff
- You're a natural athlete.
+ You ran in the rain on Tuesday.
```

Nobody can repeat a trait. They can repeat an act. This is the difference
between the durable kind of confidence and the brittle kind.

### A shortfall, completed

```diff
- You've missed 6 of your last 10 sessions.
+ You've missed six of the last ten. All six were mornings. The four you made
+ were after work.
```

The first is a verdict. The second is something they can use. Naming a
shortfall and stopping there is the most diminishing thing writing can do.

### Level to larger

```diff
- Unlimited storage. Advanced editing. Priority support. Cloud sync.
+ You can stop deleting things to make room.
```

Both true. Only one reaches into the reader's actual week. The feature stack is
volume standing in for a claim worth making.

### The reader as subject

```diff
- This screen displays your monthly spending.
+ Here's where your money went last month.
```

The subject of the first sentence is a screen, which makes the reader a
spectator to their own money.

### Pressure removed, fact kept

```diff
- Only 3 left! Order in the next 2 hours to get it by Friday.
+ Three left in your size.
```

The fact was doing the work. The clock was doing something else.

### Affectation

```diff
- Two minutes, before anything else asks for you.
+ Takes two minutes.
```

This one is mine. I wrote the first version while trying to make a two minute
setup sound like poetry, which is how affectation happens. It reads as craft
from the inside and as strain from the outside.

### Sentences that should not exist

```diff
- Press Enter to send. Hold Shift and Enter for a new line.
+
```

Everyone knows. It costs attention and returns nothing. Cut is a valid rewrite,
and often the right one.

### A full screen

Onboarding for a sleep tracker.

```diff
- Unlock your best sleep with the world's most advanced sleep tracker! You're a
- natural night owl, you just haven't optimised your routine yet. Science shows
- that consistent sleep improves everything. Simply wear your device to bed and
- our AI will analyse your patterns. Unlimited history. Advanced insights.
- Priority support. Smart alarms. 70% OFF, next 30 minutes only!

+ Most people's worst nights cluster on one weekday. You'll probably know which
+ one by Friday.
+
+ Wear it to bed. Nothing else to set up.
+
+ The annual plan is 70% less.
```

Seven changes. The trait claim went, because it builds the brittle kind of
pride. "You just haven't optimised yet" went, because that is a verdict wearing
encouragement. The unnamed appeal to science went, because a reader who checks
and finds nothing discounts everything else. "Simply" went, because it implies
anyone competent finds this easy. The deadline went and the price stayed,
because the fact survives and the clock does not.

The opening does the real work. It makes no claim about the reader, so there is
nothing to reject, and it hands them a date by which they will have their own
evidence.

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

Eighteen patterns in four banks, each with trigger words, the mechanism, and a
before and after pair.

Content: trait praise where act praise belongs, contingent regard, diagnosis
without return, concepts wearing costumes, counting where naming belongs,
promised feeling.

Position: system as subject, controlling verbs, presupposed deficiency, copulas
and transactional verbs, missing stance, premature closure.

Commercial register: urgency and scarcity, benefit stacking, superlative and
comparison, borrowed authority.

Craft: sentences that should not exist, affectation.

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

**2.1.0** Three tests hoisted to the front, because most bad sentences die at
the first one and the old version rewrote them instead. Two patterns added:
sentences that should not exist, and affectation. All examples rebuilt to be
legible to anyone, replacing ones that only worked if you already knew the
product they came from. Added the rule that a sentence carries one position, not
three, since forcing all three onto a price line is what produced the strained
writing in 2.0.0.

**2.0.0** Two modes. INHABIT added, for setting an assistant's voice rather than
editing a document. CLEAR pass folded in from humanizer with attribution.
References split out of the single file.

**1.0.0** Three positions, sixteen patterns, two-pass audit, grounding section.

## License

MIT
