# Contributing to PT/OS Workspace

PT/OS Workspace improves when people report what works, what fails, and what could be clearer. You don't need to be a programmer to contribute. A useful bug report or correction is as valuable as a code change.

## Report a Problem or Suggest a Change

[Open a GitHub issue](https://github.com/cooperman411/plain-text-os/issues) and describe the problem or suggestion. For setup failures, include:

- **Your setup:** AI product, mode or tool, storage location, and plan if it affects file access.
- **What you tried:** The step you took and what you expected to happen.
- **What happened:** The actual result, including a short, redacted error message if useful.
- **What you verified:** Whether the AI could create a file, read it, edit that same file, and confirm the update.

Plain-language reports are welcome. You don't need to diagnose the cause before opening an issue.

## What Helps Most

- **Capability corrections.** AI products and permissions change frequently. Include a link to current vendor documentation or a reproducible test, with the date and configuration. Distinguish what you tested from what a provider claims.
- **Setup problems.** If [AGENT.md](AGENT.md) led your AI to make an incorrect assumption, skip a permission check, or claim it saved something it didn't, report the exact step.
- **Documentation improvements.** Identify unclear wording in the [README](README.md), [agent instructions](AGENT.md), or [capability matrix](CAPABILITY-MATRIX.md). Suggest a shorter or more precise explanation when possible.
- **Additional platforms and storage options.** Explain how the AI reads, creates, and updates persistent files. A chat history, uploaded reference file, or manual re-upload does not qualify as Workspace file maintenance.
- **Translations.** Open an issue before starting a translation so contributors can coordinate terminology and avoid duplicate work.

PT/OS One is the separate [single-document project](https://github.com/cooperman411/plain-text-os-one). Suggestions about paste-only or upload-only assistants belong in the [PT/OS One issue tracker](https://github.com/cooperman411/plain-text-os-one/issues), rather than the Workspace issue tracker.

## Propose an Edit

You can submit a pull request if you're comfortable with GitHub. Keep changes focused, explain the reason for them, and update related references when necessary.

For capability claims, include sources and identify any limits you could not verify. Keep product requirements consistent across the README, AGENT.md, and capability matrix.

Please don't add speculative features, complicated folder structures, or new dependencies simply because they're possible. Workspace should grow in response to real needs.

## Privacy and Conduct

Assume that issues and pull requests are public. Never include personal workspace files, private conversations, passwords, access tokens, or API keys. Replace sensitive details in screenshots and logs before posting. If a secret is exposed, revoke or rotate it promptly; deleting a comment alone might not make it safe.

Be direct and respectful. The project is intended for people with different levels of technical experience, and useful criticism is welcome. Explain what needs to change and why.

There's no formal review schedule. Some suggestions may need more testing before they're incorporated.
