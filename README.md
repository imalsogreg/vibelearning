## A Claude Code plugin for learning things.

This plugin adds the `/vibelearn` slash command, which takes a single argument,
which is a single-word topic to learn or the URL or an arXiv paper.

It then generates two plans:
 1. A You-facing plan for learning that thing, including interactive chatting,
    worksheets, and progress tracking.
 2. An agent-facing plan that guides the agent through the long-term process
    of teaching you. This prevents the agent from losing the thread of the
    lesson over the countless months and sessiosn that it takes us moist-brained
    humans to learn new concepts.

## Dependencies

 - **beads** We use [beads](https://github.com/steveyegge/beads) for the internal
   planning. `bd` must be available on your `$PATH`.

## Installation

Start the `claude` CLI.

Then run

```
/plugin marketplace add imalsogreg/vibelearning
```

to install the marketplace and

```
/plugin install vibelearn@vibelearn
```

## Try it out

Now run this and start learning about the wonderful world of Neural Operators:

```
/vibelearn https://arxiv.org/abs/2108.08481
```
