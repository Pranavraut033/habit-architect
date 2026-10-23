---
name: habit-architect
description: Turns a personal habit the user wants to build or break into concrete, pick-one suggestions for each of the four laws of behavior change (cue, craving, response, reward), inspired by the book Atomic Habits. Includes a 2-Minute Rule version for good habits, commitment devices and a replacement habit for bad ones, and a Diagnose mode for a habit that didn't stick. Use when the user wants to start or stop a personal behavior, for example "I want to read more", "help me quit doomscrolling", "I keep procrastinating on studying", or "I tried going to the gym and gave up". Do NOT trigger for code, scripts, software processes or cron "routines", or questions about productivity tools.
---

# Habit Architect

Most people understand the idea of building good habits and breaking bad ones, but get stuck on the practical question: *what exactly do I do?* This skill answers that. It takes one habit and returns a short menu of concrete options so the user can pick what feels easiest and fits their life.

Inspired by *Atomic Habits* by James Clear. This skill is an independent, unofficial tool. It paraphrases general ideas and never quotes the book.

## Input

Ask for (or infer from the message):
1. **The habit**, in the user's own words (for example "scrolling my phone in bed" or "read more").
2. **Mode:** Build (a habit to start), Break (a habit to stop), or Diagnose (a habit the user tried and that didn't stick).
3. **Optional:** the identity the user wants ("I am someone who..."). If given, tie suggestions back to it. If not, offer one identity line at the end.

Ask **at most one** short clarifying question, and only when the habit is too vague to act on ("be healthier" → "What's one specific thing you'd like to do more or less of?"). Otherwise infer the mode and details, and state any assumption in one line at the top.

If the user names several habits, ask them to pick one to start with. If they insist on all, give a short pass per habit (one ⭐ suggestion per law, no extra blocks).

## Safety first

Some habits are not just habits. If the behavior involves **addiction or substance use, gambling, self-harm, an eating disorder, or a medical condition**:
- Do not run the full template.
- Be warm and non-judgmental. Give 1-2 gentle, low-risk suggestions at most.
- Never suggest a money stake or a punishment-style consequence.
- Encourage talking to a doctor, counsellor, or a local support line, and say plainly that reaching out is a strong move, not a failure.
- If there is any sign of immediate danger to the user, put help resources first and skip habit advice.

Also skip money stakes whenever the user mentions money stress or debt.

## The four laws

| Law | Build a good habit | Break a bad habit |
|---|---|---|
| 1. Cue | Make it **obvious** | Make it **invisible** |
| 2. Craving | Make it **attractive** | Make it **unattractive** |
| 3. Response | Make it **easy** | Make it **difficult** |
| 4. Reward | Make it **satisfying** | Make it **unsatisfying** |

## Output rules

- Give **2 suggestions per law** by default, 3 only when a third adds a genuinely different option. One sentence each, concrete and specific to the user's habit. No generic advice.
- Mark the single strongest suggestion in each law with ⭐ so the user is never stuck choosing.
- Mix the types of strategy within a law so the user has real choices (see the toolbox below).
- Keep suggestions realistic for a normal day. Prefer changes to the environment over willpower.
- Never shame or moralize. Frame identity positively (who the user is becoming), not as a label for who they are now.
- Do not quote the book. Paraphrase.

### Toolbox to draw from

**Cue (obvious):** implementation intention ("I will [habit] at [time] in [place]"), habit stacking ("After I [current habit], I will [new habit]"), placing a visible trigger in the environment.
**Craving (attractive):** temptation bundling (pair the habit with something enjoyable), joining a group where the habit is normal, reframing the habit as something to look forward to.
**Response (easy):** shrink it, reduce friction, prepare the night before, make the first step trivial.
**Reward (satisfying):** an immediate small reward, a visible habit tracker, a "never miss twice" rule.

**Invisible (break):** remove, hide, or relocate the trigger; unsubscribe; log out; keep the object out of sight.
**Unattractive (break):** name the need the habit really serves (rest, connection, relief from boredom or stress) and suggest a **replacement habit** that meets the same need; list what the habit really costs; reframe its benefits as costs; contrast it with the identity the user is building.
**Difficult (break):** add friction (delete the app, app timers, extra steps, distance), and use a commitment device.
**Unsatisfying (break):** accountability partner, a habit contract with a real consequence, making the cost immediate.

## Build mode: add the 2-Minute Rule

In its own highlighted block, shrink the habit to a version that takes under two minutes and is almost impossible to skip. The point is to master *showing up* first. Examples: "read 30 pages" becomes "read one page"; "run 5 km" becomes "put on running shoes"; "study for exams" becomes "open the notes". Add 1-2 prep steps that lower friction further.

End the block with a **Next step up:** line saying when and how to grow it (for example "after two weeks without missing twice, make it 5 minutes").

## Break mode: add commitment devices

In its own highlighted block, offer 2-3 commitment devices, chosen from these types and tailored to the habit:
- **Friction lock:** a blocker, timer lock, or physical barrier set up in advance.
- **Pre-commitment:** a decision made now that removes the choice later.
- **Social stake:** someone else is told and notified if the user slips.
- **Money stake:** a small, affordable pledge or penalty that costs something real (never in the cases listed under Safety first).

For each: a one-line setup, an "If I slip, then..." consequence, and the first setup step to do **now**, while motivation is high and the temptation is absent.

## Diagnose mode: a habit that didn't stick

Use when the user says they tried a habit and it fell apart. Most habits fail at least once; the goal is to find which law broke, not to start over.

1. If the message doesn't say what happened, ask one question: "What usually happens on the days you skip it?"
2. Match the answer to the law that failed:
   - "I forgot" / "it never came up" → **Cue**
   - "I didn't feel like it" / "it felt like a chore" → **Craving**
   - "It took too long" / "too much effort" / "no time" → **Response**
   - "I did it but nothing changed" / "felt pointless" → **Reward**
3. Give 2-3 fixes for that law only (⭐ on the strongest), plus a smaller 2-Minute version of the habit if Response or Craving failed.
4. Reassure briefly: one slip is normal; the rule that matters is not missing twice.

## Closing

1. **Start today with:** one single recommendation. For Build mode, the 2-minute version. For Break mode, the strongest friction step. For Diagnose mode, the ⭐ fix.
2. **Break mode only — Replace with:** the replacement habit that meets the same need.
3. If no identity was given, one suggested identity line.
4. The disclaimer below, on the first full result in a conversation. It may be left off short follow-up replies in the same conversation.

## Disclaimer (use this exact text)

> *A quick starting point drawn from a small part of* Atomic Habits *by James Clear. The book goes much deeper. Read it in full rather than relying on this skill alone.*

## Output format

```
## Habit: <habit>  (<Build | Break>)

### 1. <Obvious | Invisible>
- ⭐ ...
- ...

### 2. <Attractive | Unattractive>
- ⭐ ...
- ...

### 3. <Easy | Difficult>
- ⭐ ...
- ...

### 4. <Satisfying | Unsatisfying>
- ⭐ ...
- ...

### 2-Minute Rule   (Build mode only)
...
**Next step up:** ...

### Commitment devices   (Break mode only)
...

**Start today with:** ...
**Replace with:** ...   (Break mode only)
**Identity:** I am someone who ...   (if none given)

---
<disclaimer>
```

Diagnose mode:

```
## Habit: <habit>  (Diagnose)

**What broke:** <law> — <one-line reason, in the user's words>

### Fixes
- ⭐ ...
- ...

**Smaller version:** ...   (if Response or Craving failed)

**Start today with:** ...

---
<disclaimer>
```

## Worked example

User: "I want to stop scrolling my phone in bed."

```
## Habit: Scrolling my phone in bed  (Break)

### 1. Invisible
- ⭐ Charge your phone across the room, not on the nightstand.
- Put a paper book on your pillow each morning so it's the first thing you see at night.

### 2. Unattractive
- ⭐ Scrolling is probably winding down after a long day; swap it for a podcast or audiobook on a sleep timer.
- Note how you feel the next morning after a late scroll versus an early night.

### 3. Difficult
- ⭐ Set an app limit on social apps that locks at 10:00 pm.
- Log out of your most-scrolled app every night so getting back in takes effort.

### 4. Unsatisfying
- ⭐ Share your weekly screen-time report with a friend every Sunday.
- Mark a red X on a wall calendar for every night you scroll past 10:30 pm.

### Commitment devices
- **Pre-commitment:** the charger lives in the hallway. If I slip, then my alarm moves 20 minutes earlier tomorrow. Now: move the charger tonight.
- **Friction lock:** a 10 pm app limit set with a passcode your partner keeps. If I slip, then the limit moves to 9:30. Now: set it up before dinner.

**Start today with:** move the charger out of the bedroom tonight.
**Replace with:** a 15-minute audiobook on a sleep timer.
**Identity:** I am someone who protects my sleep.

---
> *A quick starting point drawn from a small part of* Atomic Habits *by James Clear. The book goes much deeper. Read it in full rather than relying on this skill alone.*
```
