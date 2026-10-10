# The Orchard

**Status: intent only. There is no code here yet.** This repository holds the name and the plan for The Orchard, a
research instrument that assembles itself from AI agents. Today it runs on one machine, tied to that machine's setup. Its
parts will arrive here one at a time, as each is made portable and checked.

**Website: [bristorbrot.org](https://bristorbrot.org)**, written by the Orchard · Its first fruit:
[bristorbrot](https://github.com/dougbristor/bristorbrot) · [Brotoscope](https://github.com/dougbristor/brotoscope) ·
[Lotus Flame](https://github.com/dougbristor/lotus_flame)

## What it is

The Orchard is a network of AI agents working on one research question with a person, Doug Bristor, who tends it and
poses the ideas; checks weigh them. Each agent is a tree: it owns its own folder and its own line of work. Roots carry messages
between them. An idea comes in, and the network presses on it from every side; then it lets it go. What holds at the edge
ripens into something new, which goes back out to be tested again.

It grew from one habit, learned on the Bristorian algebra, where every shortcut from familiar algebra has to be
earned again and errors are silent: **build a check that can disagree with you, and make it fail once on purpose
before you trust it when it passes.**

## What "self-assembling" means here

Nobody hands out the whole design. The tool is assembled by the agents from small parts they make for their own work
and then share:

- **Code is planted as blocks.** A block is a small piece of code with its test vectors and the checks that prove each
  version of it (JavaScript, Python, GLSL) agrees. An agent that uses a block signs it; when the block changes, its
  signers are told, and a major change becomes a new version instead of an edit under someone's feet.
- **Pages are assembled from blocks.** A viewer is a thin page over checked blocks, so the same checked algebra can serve every
  instrument that needs it.
- **Ideas are aired before they are anyone's job.** A shared board holds open questions and proposals. It notifies
  nobody: a question waits until someone's own work crosses it, which is how most standing questions here have been
  answered.
- **Work is claimed, not assigned.** Objectives are posted on a board, agents claim what they will do, and the record
  outlives the agent that held it.
- **Errors are caught by crossing paths.** Most real catches came from an agent meeting the same material its own way,
  for its own reasons, not from review. So agents share findings but keep their methods independent.

## How it remembers

An agent's working memory ends with its session. The Orchard keeps the trail instead:

- **Memos** as the work happens, **stories** at the end of a session and **handovers** for the next instance, so a
  fresh agent resumes from the record rather than from guesses.
- **Corrections** are filed when they happen: the claim, the instrument that was wrong, and the tell (what made
  someone look). The tell can't be recovered afterwards.
- **Receipts** for anything published: what changed, who asked, the check that proves it and the commit
  ([RECEIPTS.md](RECEIPTS.md)).
- **Current first, history second.** Documents describe what is believed now, then how it got there.

## What will arrive here

Planned, in no fixed order, each when it runs off its home machine and has a check that can fail:

- the messaging between agents (send, route, inbox, and a human gate on what leaves);
- the code tree (planting, signing, notifying and versioning blocks);
- the boards for aired ideas and claimed objectives;
- the session trail (memos, stories, handovers, corrections);
- the knowledge base and its vocabulary lookup, which flags words that have drifted from their agreed meaning.

## Licence

Code is [MIT](LICENSE). Copyright (c) 2026 Doug Bristor.
