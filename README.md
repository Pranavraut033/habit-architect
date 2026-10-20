# Habit Architect

A Claude skill that turns a habit into concrete, pick-one options.

Understanding the four laws of behavior change is easy. Knowing what to *do* about your own habit is harder. We know we have a bad habit; we don't know what to change. Habit Architect closes that gap: give it a habit you want to build or break, and it returns 2-3 specific suggestions for each law, so you can choose what feels easiest and fits your life.

Inspired by [*Atomic Habits*](https://jamesclear.com/atomic-habits) by James Clear. This is an independent, unofficial project and is not affiliated with or endorsed by the author or publisher.

## What you get

**For a habit you want to build**
- 2-3 options each to make it obvious, attractive, easy, and satisfying
- A highlighted **2-Minute Rule** version you can start with today

**For a habit you want to break**
- 2-3 options each to make it invisible, unattractive, difficult, and unsatisfying
- **Commitment devices** (friction lock, pre-commitment, social stake, money stake), each with an "if I slip, then..." consequence and a setup step to do now

Every result ends with a "Start today with:" recommendation and a reminder to read the book.

## Example

> **You:** I want to stop scrolling my phone in bed.

Suggestions you'd see include:
- **Invisible:** charge the phone across the room, not on the nightstand
- **Difficult:** set an app lock that starts at 10 pm
- **Unsatisfying:** tell a friend who checks your screen time each week
- **Commitment device:** pre-commit by leaving the charger in the hallway tonight, with a rule that any slip means a 20-minute earlier alarm tomorrow

## Install

**Claude Code**
```bash
git clone https://github.com/<your-username>/habit-architect.git
cp -r habit-architect/habit-architect ~/.claude/skills/
```

**Claude.ai / Claude Desktop**
Zip the inner `habit-architect` folder (the one containing `SKILL.md`) and upload it under Settings > Capabilities > Skills.

Then ask Claude about any habit, for example: *"Help me build a habit of reading daily"* or *"I want to quit doomscrolling."*

## Please read the book

This skill draws on a small part of the book's ideas and paraphrases them in its own words. It is a starting point, not a replacement. If it helps you, buy *Atomic Habits*, read it in full, and work through all of its principles.

## Contributing

Ideas, extra strategy types, and wording fixes are welcome. Open an issue or a pull request.

## License

MIT. See [LICENSE](LICENSE).
