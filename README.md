# Elucid 🔦
### *A Claude skill that teaches while it answers*

> From Latin *elucidare* — to bring into clear light

**Elucid makes Claude honest, grounded, and educational by default — for everyone, on every topic.**

---

## What is this?

When you use Claude normally, it has some annoying habits:

- Says "Great question!" before every answer (fake)
- Answers confidently even when it's guessing or using old information
- Uses technical words without explaining them
- Dumps a wall of text instead of teaching step by step
- Adds unnecessary warnings to everything

Elucid fixes all of this — permanently, for any topic — without you having
to ask every single conversation.

---

## What changes after you install it?

**Before Elucid:**
> "Great question! I'd be happy to help. The reason your phone is crashing is likely due to insufficient RAM. Random Access Memory, commonly referred to as RAM, is a type of volatile memory..."

**After Elucid:**
> "Your phone is crashing because it's running out of RAM — the temporary memory apps use while running. Here's what's happening and how to fix it..."

Same information. No fake warmth. Jargon explained naturally. Gets to the point.

---

## The three things Elucid does

**1. Teaches while answering**
Before every step or command, it explains what it is and why you're doing it.
After every result, it explains what it means. Works for any topic — not just coding.

**2. Checks facts live**
For anything that might be outdated (news, new products, current events, AI models),
it searches live instead of guessing from old data. It clearly says "I think" vs "I know."

**3. Removes the fluff**
No fake enthusiasm. No repeating your question back to you. No unnecessary warnings.
Just clear, direct explanations.

---

## How to install

### Option 1 — Claude Code (easiest if you have it)
```bash
npx skills add ypatole035-ai/Elucid
```

### Option 2 — Manual install (works everywhere including Termux)

**Step 1** — Create the skills folder on your device:
```bash
mkdir -p ~/.claude/skills/elucid/references
```
*What this does: creates a folder where Claude looks for skills*

**Step 2** — Download the skill files:
```bash
curl -o ~/.claude/skills/elucid/SKILL.md \
  https://raw.githubusercontent.com/ypatole035-ai/Elucid/main/SKILL.md

curl -o ~/.claude/skills/elucid/references/examples.md \
  https://raw.githubusercontent.com/ypatole035-ai/Elucid/main/references/examples.md
```
*What this does: downloads the instruction files that teach Claude how to behave*

**Step 3** — Restart Claude Code if it's running.

That's it. Elucid is now active.

### Option 3 — System prompt (works on Claude.ai without any install)

Copy the contents of SKILL.md and paste it as a custom system prompt in
Claude.ai settings. Elucid will be active for all your conversations.

---

## How to verify it's working

Start a new conversation with Claude and ask any question. Notice:
- No "Great question!" at the start
- Technical terms get explained naturally
- Answers are direct and educational

Or test directly:
> "What is RAM?"

Without Elucid, Claude starts with pleasantries and dumps a definition.
With Elucid, Claude explains it like a teacher using a real analogy.

---

## Termux users

If you're using Claude Code inside Termux on Android:

```bash
# Create the skills folder
mkdir -p ~/.claude/skills/elucid/references

# Download the files
curl -o ~/.claude/skills/elucid/SKILL.md \
  https://raw.githubusercontent.com/ypatole035-ai/Elucid/main/SKILL.md

curl -o ~/.claude/skills/elucid/references/examples.md \
  https://raw.githubusercontent.com/ypatole035-ai/Elucid/main/references/examples.md
```

Then restart Claude Code. Done.

---

## Troubleshooting

**Elucid doesn't seem to be working**
Make sure the files are in the right location:
```bash
ls ~/.claude/skills/elucid/
```
You should see `SKILL.md` listed. If not, repeat Step 2 of installation.

**Claude still says "Great question!"**
Try starting a fresh conversation. Skills activate at the start of sessions.

**I want to turn it off for one conversation**
Just say "ignore Elucid for this conversation" at the start. Claude will respond normally.

---

## Frequently Asked Questions

**Does this work for all topics?**
Yes. Coding, news, history, phones, science, AI — anything.

**Does this make Claude slower?**
No. It changes how Claude writes responses, not how fast it thinks.

**Does this work on my phone?**
Yes, including via Termux on Android.

**Is this free?**
Yes. MIT license. Free forever.

**Can I contribute?**
Yes! See CONTRIBUTING.md. You don't need coding skills — you can contribute
before/after examples, test the skill on your device, or translate the README.

---

## About

Elucid was built because most AI skills are made for developers.
This one is made for everyone else — the self-learner, the curious person,
the student who wants to understand what's happening, not just follow instructions.

The name comes from the Latin *elucidare* — to bring something out of darkness
into clear light. That's the goal.

**Companion project:** [llamdrop](https://github.com/llamdrop/llamdrop) —
run local AI models on any Android phone, no PC required.

---

*License: MIT — free to use, modify, share*
*Maintainer: DeVen + community*
*Version: 0.1*
[README.md](https://github.com/user-attachments/files/26689719/README.md)
