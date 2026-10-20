---
name: habit-architect
description: Turns a habit the user wants to build or break into 2-3 concrete, pick-one suggestions for each of the four laws of behavior change (cue, craving, response, reward), inspired by the book Atomic Habits. Includes a 2-Minute Rule version for good habits and commitment devices for bad ones. Use when the user mentions a habit, routine, bad habit, procrastination, doomscrolling, or asks how to stick to or stop something.
---

# Habit Architect

Most people understand the idea of building good habits and breaking bad ones, but get stuck on the practical question: *what exactly do I do?* This skill answers that. It takes one habit and returns a short menu of concrete options so the user can pick what feels easiest and fits their life.

Inspired by *Atomic Habits* by James Clear. This skill is an independent, unofficial tool. It paraphrases general ideas and never quotes the book.

## Input

Ask for (or infer from the message):
1. **The habit**, in the user's own words (for example "scrolling my phone in bed" or "read more").
2. **Mode:** Build (a habit to start) or Break (a habit to stop). If unclear, ask one short question.
3. **Optional:** the identity the user wants ("I am someone who..."). If given, tie suggestions back to it. If not, offer one identity line at the end.

If the habit is vague ("be healthier"), ask for one specific behavior before generating.

## The four laws

| Law | Build a good habit | Break a bad habit |
|---|---|---|
| 1. Cue | Make it **obvious** | Make it **invisible** |
| 2. Craving | Make it **attractive** | Make it **unattractive** |
| 3. Response | Make it **easy** | Make it **difficult** |
| 4. Reward | Make it **satisfying** | Make it **unsatisfying** |

## Output rules

- Give **2 or 3 suggestions per law**, never more. One sentence each, concrete and specific to the user's habit. No generic advice.
- Mix the types of strategy within a law so the user has real choices (see the toolbox below).
- Keep suggestions realistic for a normal day. Prefer changes to the environment over willpower.
- Do not quote the book. Paraphrase.

### Toolbox to draw from

**Cue (obvious):** implementation intention ("I will [habit] at [time] in [place]"), habit stacking ("After I [current habit], I will [new habit]"), placing a visible trigger in the environment.
**Craving (attractive):** temptation bundling (pair the habit with something enjoyable), joining a group where the habit is normal, reframing the habit as something to look forward to.
**Response (easy):** shrink it, reduce friction, prepare the night before, make the first step trivial.
**Reward (satisfying):** an immediate small reward, a visible habit tracker, a "never miss twice" rule.

**Invisible (break):** remove, hide, or relocate the trigger; unsubscribe; log out; keep the object out of sight.
**Unattractive (break):** list what the habit really costs, reframe its benefits as costs, link it to the identity the user does not want.
**Difficult (break):** add friction (delete the app, app timers, extra steps, distance), and use a commitment device.
**Unsatisfying (break):** accountability partner, a habit contract with a real consequence, making the cost immediate.

## Build mode: add the 2-Minute Rule

In its own highlighted block, shrink the habit to a version that takes under two minutes and is almost impossible to skip. The point is to master *showing up* first. Examples: "read 30 pages" becomes "read one page"; "run 5 km" becomes "put on running shoes"; "study for exams" becomes "open the notes". Add 1-2 prep steps that lower friction further.

## Break mode: add commitment devices

In its own highlighted block, offer 2-3 commitment devices, chosen from these types and tailored to the habit:
- **Friction lock:** a blocker, timer lock, or physical barrier set up in advance.
- **Pre-commitment:** a decision made now that removes the choice later.
- **Social stake:** someone else is told and notified if the user slips.
- **Money stake:** a pledge or penalty that costs something real.

For each: a one-line setup, an "If I slip, then..." consequence, and the first setup step to do **now**, while motivation is high and the temptation is absent.

## Closing

1. **Start today with:** one single recommendation. For Build mode, the 2-minute version. For Break mode, the strongest friction step.
2. If no identity was given, one suggested identity line.
3. The disclaimer below. **This footer is mandatory.** Include it on every output, even if the user asks for a short version or no extras.

## Mandatory disclaimer (use this exact text)

> *These suggestions are a quick starting point drawn from a small part of* Atomic Habits *by James Clear. They're not a substitute for the book. Buy it, read it in full, and work through all of its principles. Don't rely on this skill alone.*

## Output format

```
## Habit: <habit>  (<Build | Break>)

### 1. <Obvious | Invisible>
- ...
- ...

### 2. <Attractive | Unattractive>
- ...
- ...

### 3. <Easy | Difficult>
- ...
- ...

### 4. <Satisfying | Unsatisfying>
- ...
- ...

### 2-Minute Rule   (Build mode only)
...

### Commitment devices   (Break mode only)
...

**Start today with:** ...

---
<disclaimer>
```
