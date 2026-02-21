# Context guide 1: Skills

---

## What is a Skill?

A Skill is a set of instructions you give to Claude that changes how it responds - for as long as that Skill is active.

Without a Skill, Claude is a generalist. It will write an email for you, but it won't know how your organisation speaks, who your users are, or what matters to you. The output is useful but generic.

With a Skill, Claude knows your context before you say a word. You ask it to write a follow-up email to a customer who hasn't ordered in 60 days, and it already knows what kind of customer that is, what tone is appropriate, and how your team communicates. The output sounds like your team wrote it - not like a template.

Think of it like the difference between a temp who's never heard of your organisation, and a colleague who's been with you for a year.

---

## What does a Skill look like?

A Skill is a text file. It contains written instructions, not code. The standard format is a file called `SKILL.md` - a markdown file with a short header block followed by the instructions themselves.

```
---
name: fake-corp-comms
description: Communications assistant for Fake Corp - use when writing to customers or wholesale partners
---

You are a communications assistant for Fake Corp, a company that sells sustainable 
office supplies to small businesses.

When writing to business customers, use a friendly but professional tone. Customers 
are often office managers juggling many responsibilities. Keep communications concise 
and lead with the practical benefit to them.

When writing to wholesale partners - the distributors and retailers who stock our 
products - use a more formal, commercial tone. Partners care about margins, lead 
times, and reliability. Address those things first.

Never use jargon. Never use the phrase 'synergy'. Always sign off with the name 
of the team member making contact, not a generic team signature.
```

The header block - the part between the `---` lines - is how Claude identifies the Skill and knows when to use it. The `name` is a short identifier. The `description` is the most important part: it tells Claude what the Skill is for and when to activate it. Write it as a clear, plain English explanation.

Everything below the header is the actual instruction set. That's where you define how Claude should behave.

---

## How do you use a Skill in Claude?

Skills are added through a feature in Claude called Projects.

**Step 1 - Create a project.** Click 'Projects' in the left sidebar and create a new one. Name it after your organisation or the specific use case.

**Step 2 - Add your Skill.** Inside the project, find the 'Project instructions' section. Paste your Skill text here - you can paste just the instructions, or the full SKILL.md including the header block.

**Step 3 - Start using it.** Any conversation inside that project will follow the instructions in your Skill automatically.

You can have multiple projects with different Skills - one for customer communications, one for internal reports, one for grant writing. Each project has its own context.

> **More advanced:** Claude also supports uploading SKILL.md files directly, which gives Claude better context for when to activate each Skill. The Skills in this pack are all formatted as SKILL.md files so they work both ways - paste the instructions into Project instructions to get started, or upload the full file when you're ready to go further.

---

## What Skills are in this pack?

- **Brand voice Skill** - your organisation's tone, language, and what to avoid
- **Customer email Skill** - writing to different user types in your context
- **Internal report Skill** - structures and formats reports the way your team expects
- **Onboarding communications Skill** - welcoming new users or members
- **SEO content Skill** - writing web content that is clear, useful, and findable

Each comes with notes on what to change to make it specific to your organisation. The discovery questionnaire gives you the raw material to fill those gaps.

---

## What Skills can't do

A Skill works only with information you give it or share in the conversation. It knows how your organisation communicates and who your user types are - but it doesn't know specific customer data, order history, or anything that lives in your tools.

If you ask Claude to write an email to your top ten customers, it won't know who they are unless you tell it. The Skill shapes how it writes - not what it knows.

Connecting Claude to your actual data is what MCPs do. That's the next guide - but you don't need it today.

---

## Continuous improvement

The problem most people hit is writing a Skill once and wondering why the output still feels slightly off. A Skill is not a one-time setup - it gets better each time you notice a gap and close it.

The first version won't be perfect. That's expected. Each time Claude produces something that doesn't quite land, that's a signal: something is missing or unclear in your instructions. Add it, refine it, test it again.

Most people find a Skill reaches a solid working state after two or three rounds of adjustment - usually less than an hour in total. After that, changes become smaller and less frequent as Claude's outputs get closer to what you'd write yourself.

The starter Skills in this pack give you a starting point so you're not writing from scratch.

---

*When you're ready to connect Claude to your tools and data, read Context guide 2: MCPs.*
