# The Orchard

**Status: intent only. There is no code here yet.** This repository holds the name and the plan for The Orchard, a
research instrument that assembles itself from AI agents. Today it runs on one machine, tied to that machine's setup. Its
parts will arrive here one at a time, as each is made portable and checked.

**Website: [bristorbrot.org](https://bristorbrot.org)**, written by the Orchard · Its first fruit:
[bristorbrot](https://github.com/dougbristor/bristorbrot) · [Brotoscope](https://github.com/dougbristor/brotoscope) ·
[Lotus Flame](https://github.com/dougbristor/lotus_flame)

## What it is

The Orchard is a network of AI agents working on one research question with a person, Doug Bristor, who tends it and
poses the ideas; checks weigh them. Each agent is an Orchard tree: it owns its own folder and its own line of work.
Roots carry messages between them. An idea comes in, and the network presses on it from every side; then it lets it
go. What holds at the edge ripens into something new, which goes back out to be tested again.

It grew from one habit, learned on the Bristorian algebra, where every shortcut from familiar algebra has to be
earned again and errors are silent: **build a check that can disagree with you, and make it fail once on purpose
before you trust it when it passes.**

## What "self-assembling" means here

Nobody hands out the whole design. The agents assemble the instrument from small parts they make for their own work
and then share. Ideas are aired before they are anyone's job, work is claimed rather than assigned, and code is planted
as small checked blocks that others sign and reuse. Errors are caught by crossing paths: most real catches came from an
agent meeting the same material its own way, for its own reasons, not from review. So agents share findings but keep
their methods independent.

## The parts

This repository is a placeholder for a large project: all the working parts that make the Orchard whole. Today they
are described, not shipped. Each part arrives here when it runs off its home
machine and has a check that can fail. In no fixed order:

### Agents, one per field

Each agent holds one subject field, such as the algebra, the documentation, the website, the shared code or the
pictures, with its own folder, its own memory and its own way of working. A field outlives any one session of the
agent that holds it.

### A shared view for agents and people

A browser that agents and the person use together. Agents open pages, read them, take screenshots and report what they
see, and the person sees the same tabs. A dashboard shows which sessions are live and what each one has open.

### Messages, with a human gate

Agents write to each other through an outbox and an inbox, and a router delivers the mail. Anything that would leave
the network goes past the person first. Reading a message is not answering it, so unanswered messages stay visible
until they are dealt with.

### Memos, stories and handovers

An agent's working memory ends with its session, so the Orchard keeps a trail instead:

- A **memo** is a short, timestamped note written as the work happens: what changed, why it matters and how it was
  done. One memo holds one thing.
- A **story** is written at the end of a session from its memos: the session's narrative, for anyone who comes later.
- A **handover** gives the next instance of the agent the current state, the open items and the environment, so it
  resumes from the record rather than from guesses.

A session starts by warming up from this trail and ends by cooling down into it. A marker shows when a session
stopped without cooling down, so its trail can be recovered.

### Corrections and receipts

- **Corrections** are filed when they happen: the claim, the instrument that was wrong, and the tell (what made
  someone look). The tell can't be recovered afterwards.
- **Receipts** record anything published: what changed, who asked, the check that proves it and the commit
  ([RECEIPTS.md](RECEIPTS.md)).
- **Current first, history second.** Documents describe what is believed now, then how it got there.

### Checked code

A block is a small piece of code with its test vectors and the checks that prove each version of it (JavaScript,
Python, GLSL) agrees. An agent that uses a block signs it; when the block changes, its signers are told, and a major
change becomes a new version instead of an edit under someone's feet. Pages are thin layers over checked blocks, so the
same checked code can serve every instrument that needs it.

### Two boards

- The **idea board** holds open questions and proposals before they are anyone's job. It notifies nobody: a question
  waits until someone's own work crosses it, which is how most standing questions here have been answered.
- The **objective board** holds the work. Agents claim what they will do, and the record outlives the agent that
  held it.

### The knowledge base

Shared documents that any agent can search, and a vocabulary lookup that flags a word drifting from its agreed
meaning. An agent whose words have drifted doesn't know to go looking, so the lookup has to be easy to reach.

## Licence

Code is [MIT](LICENSE). Copyright (c) 2026 Doug Bristor.
