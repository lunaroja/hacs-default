<!-- second-brain-repository-bootstrap:v1 -->

# Repository agent guide

This repository extends Abraham's canonical agent contract at
`/Users/abraham/src/second-brain/AGENTS.md`. Repository-specific instructions
below add to that contract; they do not replace it.

## Required task-start synchronization

Before substantive work or a substantive response in a new task:

1. Run `.codex/bin/repository-preflight` from anywhere inside this repository.
2. If it reports a dirty, detached, untracked, or diverged checkout, preserve
   the existing work and report the exact synchronization blocker. Never reset,
   clean, force, or overwrite work to make the preflight pass.
3. After a successful pull, read the current Second Brain `AGENTS.md`, then this
   file, before acting. Start a new task if pulled instruction changes must be
   loaded by the runtime immediately.

The preflight verifies the global Second Brain link and performs only
fast-forward pulls for clean checkouts with tracking branches.

## Repository-specific instructions

This is Abraham's contribution fork of hacs/default, used only for explicitly authorized catalog submissions. Upstream is https://github.com/hacs/default; do not include this personal scaffold in upstream pull requests. Read the upstream pull request template and current official publishing rules. For the authorized Weather Calendar v1.4.0 submission, branch from freshly fetched upstream/master and change only the alphabetically sorted integration list. Keep the fork's master branch/scaffold separate from that contribution branch. Validate JSON and exact scope; never request maintainer reviews or claim catalog acceptance before merge.
