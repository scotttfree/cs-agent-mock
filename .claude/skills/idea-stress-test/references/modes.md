# Optional modes

All hard rules from SKILL.md still apply in every mode: numbers with assumptions, no generic advice, every criticism paired with a test or fix, search for current facts, no softened verdicts.

If the idea is too vague to evaluate, intake still comes first in every mode: ask up to 3 sharp questions before running the mode.

---

## `quick`

For when the user wants a gut check in under a minute of reading (~250–400 words).

```
## The idea in one line
(who / pain / how it makes money)

## Verdict
**[Pursue / Pivot to X / Park / Kill]** — conviction: [low/med/high]
What would change my mind: ...

## Top 3 risks
1. **[Assumption]** (Hope/Belief) — why it matters, in one or two sentences with a number if possible.
2. ...
3. ...

## One experiment
What / who / pass-fail threshold / cost — targeting risk #1.
```

End with one line: "Say `full` for the complete stress test."

---

## `partner meeting`

Simulate a VC partner meeting. Interactive: **one question per turn**. Do not dump all questions at once.

**Setup (first turn):**
- One-line restatement of the idea.
- "I'll ask ~6 questions, one at a time. I'll score each answer 1–5 and tell you why. Answer like you're in the room."
- Ask question 1.

**Question order** (adapt to the idea; skip any that are irrelevant):
1. Why is this a must-have and not a nice-to-have? Who has this problem worst?
2. Who writes the cheque, and what are they using today?
3. Walk me through how you get your first 10 customers. Names or types.
4. Bottom-up, how big can this get? Show me the arithmetic.
5. Why won't [the most obvious big player] ship this as a feature next year?
6. Why you? What do you know that others don't?
7. (Optional) What has to be true for this to be a $100M+ revenue business?

**Each subsequent turn:**
```
**Score: X/5** — one or two sentences on why. What a 5/5 answer would have included.
(Optional follow-up probe if the answer dodged the question; it counts as part of the same question.)

**Q[n]:** next question
```

Scoring rubric:
- **5** — specific, evidenced, quantified, anticipates the follow-up.
- **4** — specific and credible, minor gaps.
- **3** — plausible but asserted rather than evidenced.
- **2** — vague, generic, or dodges the question.
- **1** — no answer, or the answer undermines the case.

Hold the same standard as the pushback rules: don't inflate scores for confident delivery.

**Wrap-up (after the last question):**
```
## Partner meeting debrief
| Question | Score | Gap |
Average: X.X/5

## How the partnership would vote
(Pass / Take a second meeting / Invest — and the deciding reason)

## What to fix before a real meeting
(top 3, each with a concrete action)
```

---

## `pre-mortem`

Frame: "It's [date two years from today] and this company is dead. Here's the post-mortem."

Write in past tense, as if it happened. Be specific and plausible, grounded in this idea's actual risks rather than generic startup failure.

```
## Post-mortem: [idea name], [month year] – [month year]

### What happened
(4–6 sentence narrative: what got built, early signals, the turn, the end.)

### Cause of death
(the primary cause, one paragraph)

### Contributing factors
(3–5 bullets, each tagged with which assumption from the assumption map it falsified)

### The warning signs we ignored
(2–4 signals that would have been visible in the first 3–6 months, each with a metric and threshold)

### What would have saved it
(for each factor: the test or decision that would have caught it early, cheaply)
```

Then step out of the frame:

```
## Back to today
Probability this pre-mortem plays out roughly as written: [low/med/high], because ...
The single tripwire to set now: [metric + threshold + date] — if crossed, revisit the verdict.
```
