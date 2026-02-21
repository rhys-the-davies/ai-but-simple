# Contributing to the AI starter pack

Contributions are welcome. This guide tells you how.

---

## How this pack relates to Anthropic's Skills repo

This pack is a distribution layer on top of Anthropic's official Skills repository at github.com/anthropics/skills. We pull Skills from there, wrap them in plain-English guides, and make them accessible to non-technical users. When this pack's community builds something new and useful, we contribute it back upstream.

If you're building a new Skill, check Anthropic's repo first. If it already exists there, the contribution needed here is a guide - not a duplicate Skill.

---

## What you can contribute

- **New Skills** - a Skill for a use case not already covered here or in Anthropic's repo
- **Guides** - plain-English explanations for Skills that exist upstream but aren't yet in this pack
- **MCP connection guides** - setup instructions for tools not yet covered
- **Improvements** - better instructions, clearer examples, fixes to anything here
- **Adaptations** - versions of the pack for ChatGPT, Gemini, or other tools

---

## Skill format

All Skills in this pack follow Anthropic's SKILL.md standard. Every Skill is a folder containing a `SKILL.md` file structured like this:

```
---
name: your-skill-name
description: Plain English explanation of what this Skill does and when to use it
---

Your instructions here.
```

The `description` field is the most important part - it's how Claude knows when to activate the Skill. Write it clearly.

See Anthropic's official Skills repo for production examples of well-structured Skills.

---

## Standards

**For Skills:** Follow the SKILL.md format above. Test it in Claude before submitting. Include a short note in the PR explaining what the Skill does and what a user would customise.

**For guides:** Match the tone of the existing docs. The audience is a non-technical founder, not a developer. If they couldn't follow it, it needs more work.

**For all contributions:** If in doubt, open an issue first and describe what you're planning.

---

## How to submit

1. Fork the repository
2. Make your changes
3. Submit a pull request with a short description of what you've added and why

Not comfortable with GitHub? Open an issue describing what you'd like to contribute and someone will help get it in.

---

## Questions

Open an issue or get in touch at studio-rhys.com.
