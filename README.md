# Habit Architect

**A Claude skill that turns "I should really build/break this habit" into a short list of things you can actually do.**

Understanding the four laws of behavior change is easy. Knowing what to *do* about your own habit is harder. We know we have a bad habit; we don't know what to change. Habit Architect closes that gap: tell Claude about a habit, and it gives you a few specific options for each law, with the best one starred, so you can pick what fits your life.

Inspired by [*Atomic Habits*](https://jamesclear.com/atomic-habits) by James Clear. This is an independent, unofficial project and is not affiliated with or endorsed by the author or publisher.

## What you get

**🌱 Build a habit** ("I want to read every day")
- 2-3 options each to make it **obvious, attractive, easy, and satisfying**, with ⭐ on the strongest
- A **2-Minute Rule** version small enough to do on your worst day, plus when to level it up

**🧹 Break a habit** ("I want to stop doomscrolling")
- 2-3 options each to make it **invisible, unattractive, difficult, and unsatisfying**
- **Commitment devices** (friction lock, pre-commitment, social stake, money stake), each with an "if I slip, then..." consequence and a step to set up right now
- A **replacement habit** that meets the same need the old one did

**🔧 Diagnose a habit that didn't stick** ("I tried the gym and quit after a week")
- Works out which part broke (you forgot, didn't want to, it was too hard, or it felt pointless)
- Gives fixes for that part only, instead of starting from scratch

Every result ends with one **"Start today with:"** action.

## Example

> **You:** I want to stop scrolling my phone in bed.

You'd get something like:

- **Invisible:** ⭐ charge your phone across the room, not on the nightstand
- **Unattractive:** ⭐ scrolling is probably how you wind down; swap it for an audiobook on a sleep timer
- **Difficult:** ⭐ set an app limit that locks social apps at 10 pm
- **Unsatisfying:** ⭐ share your weekly screen-time report with a friend
- **Commitment device:** the charger lives in the hallway; if you slip, your alarm moves 20 minutes earlier
- **Start today with:** move the charger out of the bedroom tonight

## How to add it to Claude

Takes about a minute. No coding needed.

### On claude.ai or the Claude app

1. **[Download habit-architect.zip](https://github.com/Pranavraut033/habit-architect/releases/latest/download/habit-architect.zip)**. Don't unzip it.
2. Open Claude and go to **Settings → Capabilities**.
3. Turn on **Skills** if it isn't already on.
4. Click **Upload skill** and choose the `habit-architect.zip` file you just downloaded.

### In Claude Code

Paste this into Claude Code:

```
/plugin install habit-architect --marketplace Pranavraut033/habit-architect
```

### Try it

Start a new chat and try one of these:
- *"Help me build a habit of reading daily."*
- *"I want to quit doomscrolling."*
- *"I tried meditating every morning but gave up after a few days."*

## Thought process

**The gap.** Most habit advice stops at the principle: make it obvious, make it easy. That's the easy part to understand. What's hard is knowing what that means for *your* habit on a Tuesday night. I wanted a tool that goes from the principle to a specific action.

**Why a menu, not a plan.** Each law gets 2-3 options rather than one answer. What works depends on the person, and picking something you like is more likely to stick than following something prescribed. Fewer than two gives no choice, and more than three becomes another list to ignore. One option is starred so you're never stuck choosing.

**Why a 2-Minute Rule block.** For good habits, the hardest part is starting, so the skill always offers a version small enough to do on your worst day.

**Why commitment devices.** For bad habits, willpower in the moment loses to a habit that's easy and rewarding. So the skill pushes you to set up friction or a consequence *before* the temptation shows up.

**Why replace, not just block.** A bad habit usually meets a real need: rest, distraction, comfort. Block it without giving that need somewhere else to go, and it finds its way back. So Break mode always names a replacement.

**Why Diagnose mode.** Most habits fail at least once. Starting over from scratch throws away what you learned. Finding which part broke (the cue, the motivation, the effort, or the payoff) and fixing just that is faster and less discouraging.

**Why it steps back sometimes.** Some "habits" are really addiction, self-harm, or a health issue. For those, a clever trick or a money penalty can do harm. The skill keeps it gentle, skips the stakes, and points you toward real support.

**Why the disclaimer.** The skill is built on a small slice of one book's ideas, paraphrased in its own words. It's a starting point. The book has far more depth, and the footer says so on every full result.

## Testing

`skills/habit-architect/evals/evals.json` has six test prompts: build, break, a vague request, a false trigger (a cron job "routine"), a sensitive case (gambling), and a Diagnose case. Run them with Anthropic's [skill-creator](https://github.com/anthropics/skills) skill to check that changes don't break behavior.

## Please read the book

This skill draws on a small part of the book's ideas and paraphrases them in its own words. It is a starting point, not a replacement. If it helps you, read *Atomic Habits* in full and work through all of its principles.

## Contributing

Ideas, extra strategy types, new test cases, and wording fixes are welcome. Open an issue or a pull request.

## License

MIT. See [LICENSE](LICENSE).
