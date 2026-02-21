# Context guide 2: MCPs

**Read Context guide 1: Skills first and get comfortable with that before continuing here.**

MCPs require either some technical confidence or a short conversation with a developer. If that feels too soon, come back when you're ready.

---

## What is an MCP?

MCP stands for Model Context Protocol. Ignore the name.

It's a connection between Claude and another tool or system. It lets Claude read information from the tools your team already uses - your Airtable database, your Google Drive, your own platform - and use that information when you ask it questions.

Without an MCP, Claude knows only what you tell it in the conversation. With an MCP, Claude can look things up itself.

Instead of opening Airtable, finding the data you need, copying it into Claude, and then asking your question - you just ask the question.

---

## Why does this matter?

Small teams spend a lot of time on operational lookups - checking who a customer is, finding the last time someone was contacted, pulling together information from different places before doing anything useful with it.

MCPs remove that friction. Claude becomes a single place to ask questions about your business.

The bigger benefit is combining sources. Any single tool already has a search function. The change is when Claude can cross-reference all of them at once. "Which customers haven't been contacted in 90 days, and when did we last email them?" currently requires several tabs and several minutes. With MCPs connected, it's one question.

---

## What MCPs are available right now?

Some tools have MCPs ready to connect. No developer needed.

**Ready to connect today:**
- Notion
- Airtable
- Google Drive and Google Workspace
- Linear
- GitHub
- Slack (in progress)

The MCP connection guide in this pack walks you through setup for each of these.

**Everything else:**

Most CRM systems, custom-built platforms, and specialist tools don't have MCPs yet. You'll need a developer to build one. The developer brief template in this pack tells you what to ask for.

---

## Read-only vs read-write

MCPs can be set up in two modes.

Read-only means Claude can see your data but cannot change anything. Start here.

Read-write means Claude can read and make changes - updating records, creating entries, sending messages. This pack covers read-only only. Read-write is a conversation for later.

---

## How it works

An MCP server sits between Claude and your tool. When you ask Claude a question, it contacts the MCP server, which fetches the relevant data and passes it back. You ask a question and get an answer. The MCP is invisible.

The data Claude retrieves is live. The answers are as accurate as your underlying data - if your records are incomplete or out of date, that will show. MCPs make your existing data easier to access, they don't improve it.

---

## Security

When you connect a tool via MCP, Claude can access whatever that tool contains - but only what the MCP server is configured to expose. If you only want Claude to see certain tables in Airtable and not others, that can be configured.

The connection is specific to your Claude account. No one else can access your data through it.

For custom-built MCP servers, your developer controls exactly what data is exposed. The developer brief template includes guidance on scoping access appropriately.

If you have serious data security requirements - regulated industries, sensitive personal data, legal constraints - talk to whoever manages your data compliance before connecting anything.

---

## Skills and MCPs together

A Skill tells Claude how to write and what to know about your organisation. An MCP gives Claude access to live data. Together, Claude can pull your actual data and write about it the way your team would.

That's what this pack is building toward.

---

## Where to start

If any of your tools are on the list above, start there. If your most important tool is a custom-built platform, read the developer brief template first. If you're not sure, go back to your tool list from the discovery questionnaire and identify which tool your team consults most often. Start with that one.

---

*Start with the discovery questionnaire.*
