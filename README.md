# PT/OS Workspace

**Your personal AI operating system. Built around you.**

PT/OS Workspace gives your AI a collection of files it can read, organize, and maintain. These files contain your projects, priorities, preferences, and instructions, allowing your AI to continue working with information you've already provided. You control what gets saved and where it lives.

PT/OS stands for Plain Text Operating System. It starts with a few ordinary files and grows as your needs change. Your AI handles the organization and maintenance, so you can concentrate on the work.

## Which PT/OS Version Should You Use?

PT/OS comes in two versions:

- **PT/OS Workspace (this repository):** An AI-managed collection of files for ongoing projects, priorities, and workflows. Your AI needs access to persistent storage where it can read and update files.
- **[PT/OS One](https://github.com/cooperman411/plain-text-os-one):** A single portable document you can paste into an AI conversation or upload where supported. It works without file-management tools.

Choose the version that fits how you use AI. Neither requires you to start with the other.

## What Can It Do?

Suppose you're running a business, looking for a job, and managing several personal projects. PT/OS Workspace can help your AI keep those activities organized without requiring you to explain everything again each time you start a conversation.

Your workspace can include:

- **Projects:** Background information, decisions, progress, and next steps.
- **Priorities:** Current tasks, deadlines, and unfinished work.
- **Workflows:** Instructions for recurring activities, such as weekly planning, research, or email reviews.
- **Reference material:** Information, research, and documents you want to reuse.
- **Preferences:** How you like your AI to communicate, make recommendations, and handle tasks.

Your AI reads the relevant files when you need help and updates them as circumstances change. You can also move your files to another compatible AI assistant without rebuilding your entire system.

## Getting Started

Copy this instruction into your AI assistant:

```text
Help me set up PT/OS Workspace using this repository:
https://github.com/cooperman411/plain-text-os
```

Your AI will check which file-management tools it can use, help you choose where to store your information, and guide you through setup. It starts by asking what you want to accomplish, then helps you with something useful before building a larger system.

**PT/OS Workspace requires an AI that can read, create, and update files in persistent storage.** This includes some configurations of ChatGPT, Claude, Microsoft Copilot, Gemini, and AI agents such as Hermes or OpenClaw. Available capabilities depend on your AI, plan, tools, and permissions.

If your AI cannot open the repository link, copy the contents of [AGENT.md](AGENT.md) into your conversation and ask it to follow those instructions.

## What Does a Workspace Look Like?

Here's an example of a small PT/OS Workspace:

```text
My-PT-OS/
├── START-HERE.md
├── ABOUT-ME.md
├── CURRENT-PRIORITIES.md
├── PROJECTS/
│   ├── My-Business.md
│   └── Job-Search.md
└── WORKFLOWS/
    └── Weekly-Review.md
```

Each file has a specific purpose. `START-HERE.md` tells your AI how to use the workspace, while `ABOUT-ME.md` contains information you've chosen to save about yourself. The remaining files organize your current work, decisions, and recurring activities.

For example, `Weekly-Review.md` might instruct your AI to review unfinished tasks, identify approaching deadlines, and help plan the following week.

This is only an example. Your AI creates the structure based on your needs, adding files and folders when they serve a practical purpose. You might eventually have dozens of files, or you might find that five are enough.

## Where Do the Files Live?

You choose the storage location. Depending on your AI's capabilities, that could be a folder on your computer, Google Drive, OneDrive, a private GitHub repository, or an existing workspace your AI can access.

Plain text is the preferred format because it's widely supported, easy to back up, and independent of a particular application. Other formats, including Google Docs, can work when your AI has the necessary access. If you use a service-specific format, keep an exportable copy of your information.

Your AI should verify that it can read and update files in the chosen location before creating your workspace.

## Found Something Useful? Add It.

One of the more useful things you can do with PT/OS is incorporate ideas from other sources. If you discover an interesting article, GitHub repository, AI skill, or workflow, give your AI the link and ask:

```text
Review this and suggest anything useful we could add
to my PT/OS Workspace: [link]
```

Your AI can examine the material, explain how it works, and recommend ways to incorporate relevant ideas into your existing workspace. It should also identify compatibility issues, required permissions, and potential security concerns.

You approve any changes before they're added. This gives you a practical way to improve your system as you discover new methods and tools.

## Keeping Your Workspace Current

Your AI can maintain task lists, update project information, record decisions, and revise workflows as your needs change. You decide how much authority it has, whether that means approving every update or allowing routine maintenance within established limits.

Each workspace includes instructions that help another AI understand how the files are organized and how you prefer to work. If you switch AI assistants, give the new one access to your files and those instructions. It can continue working with your existing information, provided it has compatible tools.

PT/OS preserves the information you choose to save. It doesn't automatically extract previous conversations or synchronize the built-in memories of different AI services.

## Privacy and Ownership

Your personal workspace is separate from this public repository. You control where the files are stored, which AI services can access them, and what information they contain.

When an online AI reads a document, its contents may be transmitted to that service. Review its privacy practices before providing sensitive information, and keep a separate backup of your workspace, particularly if you allow your AI to make changes automatically.

Your files should remain accessible even if you stop using a particular AI service.

## Where PT/OS Came From

I spent months building my own AI operating system to help manage businesses, research, projects, a job search, and everyday work. Along the way, I studied agent frameworks, personal knowledge systems, AI memory projects, and LLM wikis, including Andrej Karpathy's work. I borrowed useful ideas and discarded a fair amount of unnecessary complexity.

That experience led to PT/OS Workspace. I wanted to make it possible for someone to build a useful personal AI system through conversation, without having to learn programming or spend weeks configuring software.

The system can be sophisticated. Using it should remain straightforward.

## Documentation and Contributions

Your AI uses the technical documentation during setup. You're welcome to read it, but you don't need to understand it to use PT/OS Workspace.

- [AGENT.md](AGENT.md): Instructions for creating and maintaining a workspace.
- [Capability Matrix](CAPABILITY-MATRIX.md): AI platforms, file-management capabilities, and limitations.
- [Contributing](CONTRIBUTING.md): How to report problems and suggest improvements.

PT/OS is an open project. If something doesn't work, is confusing, or could be improved, [open a GitHub issue](https://github.com/cooperman411/plain-text-os/issues). Include which AI you used, what you tried, and what happened. Corrections to the capability matrix are especially useful because AI capabilities and pricing change frequently.

Please keep personal information, passwords, and private workspace files out of public issues.

## License

Unless otherwise noted, the original material in this repository is © 2026 [cooperman411](https://github.com/cooperman411) and is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE.md).

You may copy, adapt, redistribute, and use it commercially. Give appropriate credit, link to the license, and indicate if you made changes.

Your private PT/OS documents and your own original information are not automatically licensed under CC BY 4.0 merely because you used this project. If you redistribute text copied or adapted from the repository, its attribution requirements still apply.
