# PT/OS Capability Matrix: Where the Files Live on Each AI System

**Checked: 2026-10-27, by public web research only. No sign-ins, purchases, or file writes.** Prices are US list prices reported in October 2026 sources; recheck at checkout. Where sources conflict or a claim could not be verified, that is flagged rather than smoothed over.

## How to read this

This matrix answers three questions for any AI system: can it use local files or not, is the person on a free or paid plan and at what level, and are they running an on-machine app or just a browser? Those three answers decide which PT/OS home fits.

Every system falls into one of three tiers, and the tier decides the PT/OS design:

- **Tier A, true folder:** the AI can read and write a real folder across sessions (desktop agent apps, some cloud computers).
- **Tier B, cloud container:** the AI keeps files inside its own app (Projects, Libraries, Drive/OneDrive folders) but there is no live sync with a folder on the user's disk.
- **Tier C, carry-along only:** no persistence at all; the user pastes or uploads one file every session and copies revisions back by hand.

The ladder runs from a free anonymous user (Duck.ai, Leo signed out: paste-in only) through free accounts (Projects and containers) and paid chat (bigger containers), to desktop apps (local folder) and agent workspaces (OpenClaw, Hermes Agent: the workspace is the folder), up to a seasoned git or Obsidian user (repo or vault as the home). The universal fallback that works on every system in this matrix is a single 1-page START HERE file, pasted or uploaded each session. The per-system sections below say what each system adds on top of that.

---

## 1. ChatGPT (OpenAI)

**Plans:** Free $0; Go $8/mo; Plus $20/mo; Pro $100/$200/$500/mo; Business $20/user/mo annual. Student: no standing discount; a time-limited US offer gave verified students 4 free months of Plus (claim by Oct 31, 2026). Everyday text chat reported as unlimited on Free/Go/Plus/Pro since Aug 2026; Work/Codex metered separately.

**1. Files across sessions?** Yes, Tier B. Projects (web/mobile/desktop, all plans) hold chats, instructions, and uploaded files persistently. Chat history and memory also persist, but memory is not a file folder. Project files are uploaded copies, not a live link to a disk folder; edits on disk do not reach the project copy.

**2. Local computer folder?** Yes, but desktop app only, Tier A. Requires the new unified ChatGPT desktop app (macOS/Windows); the old app is now ChatGPT Classic without the new agent features. In Work or Codex, open/attach one local folder and grant access to that folder only; it can read and write inside it. Work is limited and desktop-only on Free/Go, full on Plus/Pro. Codex full access starts at Plus. Local work needs the computer awake with the app open; web/mobile Work runs in the cloud and cannot read local files. Grant only the PT/OS folder, start on Ask for approval. (Standalone Codex app folded into the desktop app July 9, 2026; Atlas browser retired Aug 9, 2026.)

**3. Cloud documents?** Yes. Connected Apps cover Google Drive, SharePoint/work-or-school OneDrive, Dropbox, Box. Work can search/read Drive files and is reported to create, update, move, share, and delete Drive files with confirmation. SharePoint coverage is work/school OneDrive, not personal OneDrive. No native iCloud connector found; workaround is iCloud Drive synced to the local machine, then desktop Work on the synced copy.

**4. PT/OS home and simplest path:**
- Non-technical web/mobile user: one consolidated file (e.g. `PT-OS-START-HERE.md`) uploaded to a ChatGPT Project, plus the same text in Project instructions. Stay under the file cap (5 Free, 25 Plus, 40 Pro/Business). When it changes, delete and re-upload; do not assume in-place editing.
- Desktop user: folder `Documents/PT-OS`, opened in Work (Plus for full access).
- Cloud-first user: PT/OS folder in Google Drive, connected to ChatGPT, used via Work. Not a true live sync into Projects.

**Limits that matter:** Projects: 5 files Free, 25 Go/Plus, 40 Pro/Business; max 10 files uploaded at once; per-file limits reported at 512 MB documents, 2M tokens text, ~50 MB spreadsheets, 20 MB images. Work/Codex on Plus/Business metered in a rolling 5-hour window plus possible weekly limits.

**Unverified:** whether ChatGPT can edit an uploaded Project source file in place (evidence points to replace/re-upload, not confirmed in-place editing); personal OneDrive write behavior beyond SharePoint/work-school scope.

**Sources:** https://stashbase.ai/blog/chatgpt-desktop-vs-web/ · https://www.developersdigest.tech/blog/chatgpt-work-vs-claude-cowork-2026 · https://community.openai.com/t/feature-request-allow-direct-in-browser-editing-of-text-files-in-chatgpt-project-sources/1395282

---

## 2. Claude (Anthropic, incl. Cowork and Claude Code)

**Plans:** Free $0; Pro $20/mo ($200/yr); Max 5x $100/mo; Max 20x $200/mo; Team Standard $25/seat/mo ($20 annual). Student: no individual student discount found; Claude for Education is bought by the institution. A 7-day guest pass from a Pro/Max subscriber is reported as the closest trial route.

**1. Files across sessions?** Yes, Tier B. Chat Projects (all plans; Free capped at 5 projects, Pro/Max unlimited) hold persistent knowledge files and custom instructions. Cowork Projects (paid) add instructions, scheduled tasks, context sources, and memory. Artifacts can be downloaded but are not a persistent folder.

**2. Local computer folder?** Yes, paid only, Tier A with a recent change. Claude Cowork (Pro/Max/Team/Enterprise) in the Claude Desktop app (macOS/Windows; Linux beta) can read, write, and create files in folders you specify, with Manual/Auto/Skip permissions; start on Manual. **Change, Oct 6, 2026: new Cowork tasks on Pro/Max now run in the cloud and the "Only on your computer" option was removed.** Local file reach now requires Claude Desktop open, fetching a copy of just the file needed. Claude Code (paid, terminal/IDE/desktop) runs in the folder you start it in with true local read/write and reads a `CLAUDE.md` briefing file; this is Anthropic's pointed-to route for strict stay-on-this-computer work, but it is technical, not the non-technical default.

**3. Cloud documents?** Yes, with nuances. Google Drive/Workspace connector: search Drive, read Docs/Sheets/Slides/PDFs, create/upload files, and per Anthropic help summaries create folders, share, move, trash, and edit Docs/Sheets/Slides, with approval before each action. One detailed test notes Claude can read a Sheet and save a new spreadsheet but cannot edit an existing Sheet cell by cell. Microsoft 365 connector searches SharePoint, OneDrive, Outlook, Teams; requires work/school account plus admin consent; personal OneDrive not supported; writes off until admins enable them. No native iCloud connector; workaround is a locally synced iCloud Drive folder as the Cowork/Code working folder.

**4. PT/OS home and simplest path:**
- Non-technical free user: one consolidated file uploaded to a Claude Project (max 5 projects on Free), plus project instructions. Re-upload when it changes.
- Paid user: Pro + Claude Desktop, one folder `Documents/PT-OS` linked to a Cowork project, only that folder granted, Manual approvals. Expect cloud execution with local reach only while Desktop is open; keep a master copy.
- Cross-device paid user: PT/OS folder in Google Drive via the Drive connector, accepting per-action approvals. For phone-only users, the Project single-file route is still simpler.
- Technical alternative: Claude Code in the PT/OS folder with a `CLAUDE.md` start-here file.

**Limits that matter:** Usage is not a fixed message count (Pro described as at least 5x Free per 5-hour window; Free roughly tens of messages per window in independent reports). Project files reported at 30 MB each; paid retrieval mode expands effective capacity ~10x when project knowledge nears context limits.

**Unverified:** Google Workspace connector availability on Claude Free (sources conflict); in-place editing of Chat Project knowledge files (evidence points to replace/re-upload); status of the old Desktop Filesystem MCP route under the merged Sept-Oct 2026 Cowork UI.

**Sources:** https://learn.techwithdarin.com/guides/claude-cowork/index.html · https://aiunderstanding.org/news/anthropic-transitions-claude-cowork-to-cloud-based-execution · https://www.usecarly.com/blog/can-claude-edit-google-sheets/

---

## 3. Google Gemini (incl. Spark, Antigravity)

**Plans:** Free $0 (15 GB Drive); AI Plus $4.99/mo (400 GB); AI Pro $19.99/mo (5 TB); AI Ultra $99.99/mo entry and $199.99/mo top tier (20 TB). Student: eligible US college students get AI Pro free for 12 months; eligible students in 140+ other markets get AI Plus free for 12 months; redeem by Dec 31, 2026, via SheerID. Free-tier limits moved in 2026 from fixed daily caps to compute-based limits refreshing about every 5 hours up to a weekly cap.

**1. Files across sessions?** Yes, Tier B. Chat history persists; Gems are saved custom assistants with instructions and reference files (free and paid); Notebooks (formerly NotebookLM, rolled into the Gemini app April 2026, free on web) hold chats, files, sources, and instructions persistently; Canvas is a persistent editable document/code workspace with one-click export to Google Docs. Gap: no browsable plain-text folder inside Gemini itself; the durable copy must live in Drive.

**2. Local computer folder?** Mostly no. Web/mobile: no local access, upload per prompt. **Gemini Spark on Mac: yes, but only for folders explicitly added as Connected folders in the Gemini Mac app sidebar, revocable.** Requires Apple silicon Mac on macOS Sequoia (15.0)+, Mac available with the app running for local tasks. Spark launched June 30, 2026, initially reported as Ultra only, US only, 18+; later Oct 2026 guides describe Pro or Ultra eligibility. Windows app launched Sept 10, 2026, but local-folder access is still reported Mac-only. **Antigravity** (separate developer product, free download, macOS/Windows/Linux) opens a real local folder as a workspace with full read/write, but it is a VS Code-style IDE, not the non-technical path.

**3. Cloud documents?** Yes for Google Drive, with limits. A Gem holds up to 10 files at a time, up to 100 MB each; Docs/Sheets added to a Gem are reported to auto-recognize latest updates, while other uploaded file types need re-upload after changes. Gemini in Drive/Docs can create a Doc/Sheet/Slides file, save to Drive, export chat output to Docs/Sheets, and edit inside an open Doc with accept/reject. No native iCloud or OneDrive PT/OS path verified.

**4. PT/OS home and simplest path:** Put PT/OS in Google Drive, not on local disk and not only in Gemini chat memory. Create a Drive folder `PT-OS`; make one master file the system of record, preferably a Google Doc called PT-OS Start Here (consolidated, because of the 10-file Gem limit); create one Gem called PT-OS with the core instructions pasted in and the master Doc attached, or a Notebook with the master Doc plus key files. Each session, open that Gem/Notebook, not a blank chat. Edit the Doc in Drive when things change; keep a downloadable .md/.txt copy in the same folder as a portable backup, but do not expect Gemini web chat to edit that backup in place.

**Limits that matter:** Gem: 10 files, 100 MB each. Free Drive storage 15 GB.

**Unverified:** whether Spark on Mac is open to Pro or still Ultra only (sources conflict); reliable in-place editing session after session of a single .md/.txt file in Drive from Gemini web chat; any native iCloud path.

**Sources:** https://www.aiagentslibrary.com/blog/gemini-spark-mac/ · https://workspaceupdates.googleblog.com/2024/11/upload-google-docs-and-other-file-types-to-gems.html · https://www.digitaltrends.com/computing/all-gemini-users-can-now-access-notebook-projects-on-the-web-without-paying-a-dime/

---

## 4. Grok (xAI, incl. Grok Bot)

**Plans (X Subscription bundle since Oct 12, 2026, covering Grok, Grok Bot, Cursor, X):** Free $0 (limited chat/agent requests; Grok Bot not included); Plus $8/mo ($80/yr); Premium $30/mo ($300/yr, 4x Plus usage, lowest tier including Grok Bot); Super $100/mo; Ultra $200/mo; Teams per-seat at Premium/Super/Ultra prices. No student plan found. xAI does not publish a message count for the shared weekly pool.

**Warning: two different products.** The Grok chatbot (grok.com, Grok app, X) is chat only. Grok Bot is a separate agent product with a persistent cloud computer. Do not conflate them.

**1. Files across sessions?** Chatbot: yes, limited, Tier B. Chat history persists, cross-conversation memory can be turned off, and Projects/Workspaces attach files and custom instructions that apply to chats inside that Project; uploaded files become persistent context for that Project. Grok Bot: yes, strongly, Tier A (cloud). A named Bot keeps role, memory, preferences, files, browser sessions, and routines across sessions and keeps working after the laptop closes. Caveat: all Bots on one account share one persistent cloud computer; files, sessions, and credentials are visible across Bots, and deleting a Bot does not necessarily delete its files or logins. Separate Bots are explicitly not a security boundary.

**2. Local computer folder?** Chatbot alone: no; uploads are per session or per Project, not live SSD access. Grok Bot: yes, but opt-in and approval-gated, not the default. Via the Grok Bot desktop app (macOS/Windows/Linux, plus mobile clients), a Bot can run commands on a registered local computer, read local files, and move files to/from its cloud computer. Documented default is "Ask every time" for local execution; xAI docs reportedly recommend "Never allow" unless a Bot has a specific reason to work on local files. Not a seamless "watch my PT/OS folder" sync.

**3. Cloud documents?** Read/search yes; write selectively. Built-in connectors (available to all Grok users, with an extra admin step on Business/Enterprise) include Gmail, Google Calendar, Google Drive, OneDrive, Outlook, Teams, SharePoint, Salesforce, plus GitHub, Notion, Box, Canva, and others, many via MCP. Strongest verified write path is GitHub: a free-tier test reported connecting GitHub and having Grok search repos, explore file trees, and push files via GitHub's remote MCP server, making a private GitHub repo a plausible live PT/OS home. iCloud is not listed among built-in connectors.

**4. PT/OS home and simplest path:**
- Paid route ($30/mo Premium+): Grok Bot's cloud computer as the durable home. Install the desktop app, create one Bot, tell it to keep PT/OS in its persistent cloud workspace (secondary sources cite `/workspace`), start every PT/OS task with that Bot. Leave local execution off or on Ask every time; use the cloud copy as master.
- Low-cost route: one Grok Project called PT/OS, core instructions in Project instructions, PT/OS files uploaded (one master .md simplest), always start PT/OS chats inside that Project. Keep a backup on the user's computer or in Drive/GitHub; a Project is a Grok-internal container, not a Finder/Explorer folder.
- Portable route (least non-technical): private GitHub repo connected via Grok Connectors; Grok reads and updates files in the repo.

**Limits that matter:** Free tier is limited chat/agent requests with unpublished counts. Project gating on Free/Plus under the new X Subscription was not confirmed in an official page; older reporting said SuperGrok Lite excluded Projects. Do not promise Projects on Free.

**Unverified:** a general reliable two-way edit loop for Google Drive or OneDrive plain-text files (open a Drive .md, edit in place, save back); connector pages are framed mainly around opening, browsing, and searching.

**Sources:** https://docs.x.ai/grok/connectors · https://teamvoy.com/blog/what-is-grok-bot/ · https://launchdock.app/en/articles/grok-connect-github/ · https://www.grokbotwiki.com/guides/what-is-grok-bot

---

## 5. Microsoft Copilot (incl. Copilot Cowork)

**Plans:** Copilot free $0 (basic chat, daily limits, no Copilot inside Office desktop apps). Microsoft 365 Personal $9.99/mo; Family $12.99/mo; Premium $19.99/mo ($199.99/yr, up to 6 TB shared OneDrive); Pro (consumer) $99.99/mo. Standalone Copilot Pro ($20/mo) stopped selling to new customers Oct 2025; support ended Aug 2026. Business Copilot $21/user/mo annual (reported discounted to $18 through Dec 31, 2026); Enterprise $30/user/mo annual. Student: no universal free year verified; the Ultimate College Bundle free-year offer closed Aug 31, 2026; current live paths found were 50% off Microsoft 365 with Copilot (reported Personal at $4.99/mo) and Copilot Chat at no extra cost where the school holds eligible Education A1/A3/A5 licenses. (GitHub Copilot is separate and free for verified students, but it is a coding tool, not consumer Copilot.)

**1. Files across sessions?** Yes, but the useful persistent constructs are paywalled for personal accounts, Tier B. Chat history persists when signed in. Copilot Pages (dynamic persistent canvas) requires a Microsoft 365 Personal/Family/Premium/Pro subscription for personal accounts (work/school accounts with SharePoint/OneDrive storage get it without a Copilot license). Copilot Notebooks are scoped workspaces with specific references; third-party comparisons report up to 300 files but only the first 100 references used for grounding. Memory controls exist but are not a visible PT/OS folder.

**2. Local computer folder?** No, for the agent paths that matter. Microsoft Learn's Cowork FAQ states it directly: Cowork cannot access or edit files stored locally on the device; it works with files in OneDrive and SharePoint, cannot delete OneDrive/SharePoint files or folders, cannot read encrypted files, and attachments must be under 200 MB. Consumer Copilot web/app has no verified persistent local-folder access (one guide reports up to 20 files per conversation, 50 MB each, auto-deleted after no more than 18 months). The one local exception is not file access: Cowork can use the local Edge browser for automation, off by default, admin-activated. Practical workaround: OneDrive sync mirrors the OneDrive PT-OS folder to the PC for local editing, and Copilot reads the cloud copy.

**3. Cloud documents?** Yes, depth depends sharply on license. Paid Microsoft 365 Copilot can ground in OneDrive/SharePoint files the user has permission to access and work inside Word, Excel, PowerPoint, Outlook, Teams. Free Copilot Chat cannot autonomously open SharePoint files, edit a OneDrive file, search Teams, or read Outlook mail; the user must upload the file each time. Copilot in OneDrive/SharePoint was announced at an Oct 20, 2026 event as able to work across selected files, reorganize folders, and save repeatable personal skills as Markdown files, but one admin-notice report says it was in public preview late Aug to late Sept 2026 with general availability targeted late Dec 2026, so GA is not confirmed as of Oct 27, 2026. OneDrive now opens, edits, and co-authors HTML and Markdown files while keeping the underlying .md intact. Google Drive/Gmail/Docs connections for consumer Copilot were mentioned in one third-party guide but read/write PT/OS behavior was not verified.

**4. PT/OS home and simplest path:**
- If the user already has Microsoft 365 Personal/Family/Premium or a work/school account with OneDrive: OneDrive folder `PT-OS`; one master file, preferably `PT-OS.md` (Markdown now natively editable in OneDrive) or a Word doc; one Copilot Notebook with that master file (and only the most important references) added; start PT/OS sessions from that Notebook. Turn on OneDrive sync for local editing. Do not expect Copilot to delete, reorganize, or rewrite the whole folder on its own, and do not expect Cowork without a paid business Copilot license plus a credit budget.
- If the user is on free Copilot only: same OneDrive folder and single master file as the durable copy, but accept upload/attach-each-session, because free Copilot Chat does not persistently ground in OneDrive. Do not buy Cowork or E7 for personal PT/OS; cost and admin setup are disproportionate.
- Cowork specifically (for completeness): multi-step agent, requires a Microsoft 365 Copilot seat (Business $21 or Enterprise $30/user/mo), and since GA June 16, 2026, task execution is billed separately in Copilot Credits at $0.01/credit pay-as-you-go (third-party estimates: light tasks ~$1-3, heavy ~$7+). Cowork sessions are tasks, not projects; custom skills are stored as SKILL.md files but are not validated by Microsoft.

**Limits that matter:** Cowork attachments under 200 MB; consumer uploads ~20 files/conversation, 50 MB each, auto-deleted within 18 months; Notebooks ~300 files, first 100 used for grounding.

**Unverified:** Copilot in OneDrive/SharePoint GA status (targeted late Dec 2026); in-place repeated editing of a single .md in OneDrive by consumer Copilot chat; any native iCloud Drive path; exact current student pricing.

**Sources:** https://learn.microsoft.com/en-us/copilot/microsoft-365/cowork/cowork-faq · https://support.microsoft.com/en-us/microsoft-365-copilot/how-microsoft-365-copilot-pages-works · https://core.iiankehn.com/posts/onedrive-copilot-html-markdown.html

---

## 6. Mistral (Le Chat, now Vibe)

**Recent change: on May 28, 2026, Mistral renamed Le Chat to Vibe** and merged it with its coding agent. Same address (chat.mistral.ai), same account, existing conversations carry over. Older "Le Chat" guides describe the same product.

**Plans:** Free $0 (limited messages/web searches, image generation, 100+ connectors, voice, project folders; Mistral does not publish a free message count, and older "about 25 messages/day" claims should not be treated as vendor-confirmed). Pro $14.99/mo US before tax (up to 6x more messages, 5x more web searches, 40x more images than Free, 15 GB libraries, Code Interpreter, CLI/IDE coding tools). Student $5.99/mo verified, with Pro features. Team $24.99/user/mo, 2-user minimum (shared workspace, 30 GB/user, knowledge connectors). Enterprise custom.

**1. Files across sessions?** Yes, Tier B, the strongest of the smaller systems here. Account-based conversation history, Projects grouping chats/files/tools/settings, Libraries collecting documents, a Canvas editor for drafting/editing deliverables, and a Knowledge Base/memory feature for preferences and context. Uploads include PDF, Word, PowerPoint, Excel, CSV, plain text, Markdown, code, and common images. Privacy note: on individual Free/Pro/Student plans, conversations are used for training by default, with an opt-out toggle in Privacy settings; data accessed through connectors is stated not to be used for training.

**2. Local computer folder?** No in normal web/app chat; no live sync with an SSD folder. Uploads go into a Project/Library individually, and edited Canvas output must be downloaded and saved back to the master copy by hand. Automatic write-back to a local folder was not verified. Technical exception: Vibe Code (Pro+) has read/write filesystem access against a local checkout via CLI or VS Code extension, but Mistral's docs say Vibe Code is built primarily for source-code work while Vibe Work fits documents/business tools; not a non-technical PT/OS path (needs Pro, terminal or VS Code, local project folder).

**3. Cloud documents?** Read/search yes, with caveats; two-way live editing not verified. Work-mode connectors listed include Gmail, Google Calendar, Outlook, Slack, Notion, GitHub, SharePoint, Box, Linear, Stripe, Atlassian, plus custom MCP connectors. Enterprise search starts with Google Drive, SharePoint, OneDrive, Google Calendar, Gmail. Team adds knowledge connectors; Work mode routes outputs to Notion or SharePoint. What could not be verified: that a free or Pro consumer can connect a personal Drive folder, have Vibe notice a changed .md, edit that same file in place, and save it back. Treat Drive/SharePoint access as search/read plus task output routing, not proven live PT/OS folder sync.

**4. PT/OS home and simplest path:** Inside Vibe as a Project + Library, with the master copy kept outside Vibe. Create a free account at chat.mistral.ai; create a Project called PT/OS; upload core files to the Project's Library, starting with one short START HERE file, then workflows; add key preferences as custom instructions/Knowledge Base entries if available. When Vibe revises a workflow, download the revised version, replace the master copy on the computer or Drive, and re-upload. Vibe is the working copy, not the only copy. True local-folder editing is the Pro + VS Code step-up, not the starter path.

**Limits that matter:** Secondary source reports up to 100 files per library at up to 1 GB each; that exact current limit could not be verified on an official Mistral page, so treat as reported, not confirmed.

**Unverified:** exact free message count; exact current library file count/size limits; whether consumer Drive access edits a .md in place.

**Sources:** https://help.mistral.ai/en/articles/347583-what-kinds-of-documents-can-i-upload-to-my-libraries · https://docs.mistral.ai/vibe/code/overview · https://mistral.ai/news/le-chat-enterprise/

---

## 7. Brave Leo (built into the Brave browser)

**Plans:** Free $0, no account or login required; rate-limited access to rotating models (Llama, Qwen, Claude Haiku-class). Leo Premium $14.99/mo or $149.99/yr (~$12.50/mo annualized), usable on up to 5 devices; stronger models, higher rate limits, priority access. No student plan found. Premium does not add a cloud workspace, cloud history sync, or a Drive connector; it buys models and limits only.

**1. Files across sessions?** Only locally, on one device, limited, Tier C+. Leo can save and revisit conversations locally on the device, and its Memories/personalization feature stores facts and preferences on the device, not on Brave's servers. Temporary chats are not logged. No server-side project, library, or workspace to revisit from another computer; a Brave Community thread notes Leo memories/personalization do not currently sync across devices. Uninstalling Brave or losing the device risks losing that local history.

**2. Local computer folder?** No. No folder access, folder watching, or write-back to a local folder. In a single chat it can summarize/analyze the open tab (including PDFs and Google Docs/Sheets open in other tabs), attach a PDF (desktop and Android, Brave 1.84+), and attach PDFs/images in newer versions. Bring Your Own Model (e.g. via local Ollama) is local inference, not Leo reading/writing the user's PT/OS folder. December 2025 "Skills" (saved prompt shortcuts) and experimental AI Browsing mode in Nightly are also not a file workspace.

**3. Cloud documents?** No connector, no write-back. Only indirect path: open the Google Doc/Sheet in a Brave tab and ask Leo about that tab, or download it and attach the PDF. Leo cannot edit that Doc/Sheet in place or save back to Drive, OneDrive, or iCloud.

**4. PT/OS home and simplest path:** On the user's computer as an ordinary folder; Leo is only a reader of pasted or attached context. Install Brave (free); keep one PT/OS folder on the computer led by a single short START HERE text file; at the start of a Leo session, paste that START HERE text into Leo (or attach the one PDF); optionally add a few durable facts manually in Leo Settings > Leo > Memories (device only, editable/deletable). When Leo produces a revised workflow, copy it out of Leo and save it over the master file by hand. Most private option of this set, but worst for "the AI remembers my system" across devices or sessions.

**Limits that matter:** Free is rate-limited with rotating models; no sync across devices.

**Unverified:** whether a plain .txt/.md file can be attached the same way a PDF can; official pages emphasize PDFs and images.

**Sources:** https://brave.com/leo/ · https://brave.com/whats-new/leo-memories/ · https://brave.com/whats-new/desktop/

---

## 8. DuckDuckGo Duck.ai

**Plans:** Free $0, no account or sign-up required; daily usage limits exist but DuckDuckGo does not publish an exact number (reviewers describe limits as vague/unpredictable). Plus $9.99/mo or $99.99/yr (advanced models plus VPN, Personal Information Removal, Identity Theft Restoration; there is no AI-only subscription). Pro $19.99/mo or $199.99/yr (top models, extended reasoning, 2x Plus limits). No student plan found. Model lineups rotate by tier and over time.

**1. Files across sessions?** Effectively no, Tier C. No Projects, Libraries, workspaces, or persistent memory. Chat history is kept locally on the device/browser by default, can be deleted individually or cleared, and one source reports automatic removal after 30 conversations. An optional end-to-end encrypted Sync & Backup exists, but that syncs chats, not a PT/OS workspace. An Oct 2026 feature lets a user share a chat via an encrypted link (48 hours default, or 1/7/30 days), but uploaded files are excluded from shared chats; that is sharing, not storage.

**2. Local computer folder?** No. Web chat (plus DuckDuckGo browser/app); no desktop workspace app, no local folder access, no write-back to a local file.

**3. Cloud documents?** No. No Google Drive, OneDrive, iCloud, Notion, or other connector, and no workspace integration. A July 2026 third-party policy summary states this explicitly: no memory feature, no third-party connectors, no workspace integrations. No vendor evidence contradicting that was found as of Oct 27, 2026.

**4. PT/OS home and simplest path:** Outside Duck.ai entirely; Duck.ai is a disposable, private chat window fed by copy-paste. Keep the PT/OS master folder on the user's computer or in their own cloud drive; keep one 1-page plain-text START HERE file as the carry-along version; paste that whole file into the chat at the start of each session; copy any revised workflow out of Duck.ai and save it over the master file by hand. Paying for Plus/Pro buys stronger models and higher (still unpublished) limits only; it does not buy persistence, projects, or file access.

**INPUT LIMITS, verified by a live test Oct 27, 2026:** Duck.ai accepts a PDF up to 15 pages AND up to 5 MB. Both limits apply independently: a 16-page PDF is rejected even at 1 MB, and a 10-page PDF is rejected at 5.1 MB. This supersedes earlier third-party reporting that file uploads were unsupported. Design implication: a 1-page PT/OS PDF fits comfortably within both limits, making PDF a viable universal distribution format for Duck.ai. URL reading also worked in that live test (Duck.ai read and summarized the PT/OS repo URL), though it is not a documented input method.

**Limits that matter:** Daily limits unpublished and described as unpredictable; chat history auto-removal reported after 30 conversations.

**Sources:** https://duckduckgo.com/duckduckgo-help-pages/duckai/ai-chat-privacy · https://www.techradar.com/pro/duck-ai-review · https://spreadprivacy.com/duck-ai-private-chat-sharing/

---

## 9. Perplexity (incl. Computer and Portable Computer)

**Plans:** Free $0 (unlimited quick searches, small daily allowance of Pro searches and Deep Research, limited file uploads, free Comet browser). Pro $20/mo ($200/yr). Education Pro $10/mo for verified students/educators via SheerID, with the Pro feature set. Max $200/mo ($2,000/yr, reported web-only). Enterprise Pro ~$40/seat/mo; Enterprise Max ~$325/seat/mo, normally via contact sales.

**1. Files across sessions?** Yes, as Projects (formerly Spaces), plus thread history and a Memory setting, Tier B. A Project bundles threads, uploaded files, custom instructions, and linked context in one revisitable container; custom instructions reported at up to 8,000 characters. Files uploaded to a Project persist for later chats inside that Project; Projects can be shared with contributors on paid plans. This is not a general filesystem: the AI reads uploaded files and answers from them, and Labs on Pro/Max can generate new reports/spreadsheets/small apps as outputs. It does not automatically become the AI's memory in every new thread outside that Project. Free-tier Project access is inconsistently described (some sources say limited Spaces on Free, others say Spaces are paid-only); treat Free Projects as trial-only, not a reliable PT/OS home.

**2. Local computer folder?** Standard web/app: no, uploads are manual per file/session. Cloud Perplexity Computer: no local access by design (cloud sandbox; cannot access local files or locally installed desktop apps). **Portable Computer / Personal Computer: yes, on paid plans and qualifying hardware only, and this is a recent change.** Originally (Feb 2026) Computer was cloud-only. In April 2026, Personal Computer launched for Mac (Mac mini recommended, macOS 14 Sonoma+), initially for Max subscribers. By Sept-Oct 2026, Portable Computer expanded to Windows and to Pro as well as Max: Windows PCs with NVIDIA GeForce RTX/RTX PRO GPUs with 24 GB+ VRAM, or AMD Ryzen AI Max Series processors, via the Perplexity Windows app; and Apple-silicon Macs for on-device runs. Perplexity's own blog/LinkedIn summaries say Portable Computer runs in the Perplexity app, works with local files and connected apps, does not consume Computer credits for fully local work, and asks permission before sending content to the cloud. Not available on Free. For a non-technical user this is the worst "simplest path" unless they already own qualifying hardware; a typical laptop does not qualify.

**3. Cloud documents?** Read/search yes, but tier-gated and largely copy-based, not live two-way editing. Perplexity's official File Connectors help page (updated Oct 14, 2026), framed for Enterprise Pro/Max, lists Google Drive, OneDrive, SharePoint, Dropbox, Box; files can be searched, attached to a query, or imported into Projects. Crucially, content imported into a Project is copied at import time and stays as it was; importing again is how later changes arrive. Standard Search queries the connected service live but does not copy files into a Perplexity index. A separate official Pro-subscriber help page lists Google Drive and Dropbox connectors for Pro but says file syncing is not supported on Pro: changes in the original file do not transfer to the attached copy; the user must re-upload. Perplexity's own Drive connector page states Perplexity does not modify Drive file content, even though the OAuth scope includes edit/create/delete for sync metadata. So Drive/OneDrive/Dropbox/Box are a read source and backup location, not a live editable PT/OS folder. No iCloud connector found. Computer (cloud agent) adds broader app connectors (Gmail, Drive, Notion, Slack, Salesforce, HubSpot), but those are agent task connectors on Max, or Pro with purchased/promotional credits, not general PT/OS file sync.

**4. PT/OS home and simplest path:** One Project, one master file, plus a Drive backup the user owns. Pay for Pro ($20/mo, or $10/mo Education Pro if eligible); do not build PT/OS on Free. Create one Project called PT/OS; upload a single master file (e.g. PTOS.md) plus only the handful of workflow files actually used (stay well under the reported 50-file Pro limit); paste core operating rules into the Project's custom instructions; always start PT/OS work inside that Project, never in a fresh general thread; keep the true master copy in Drive or on the computer and re-upload/re-import after edits, because the Project copy is a snapshot and will go stale. If the user already has qualifying hardware and Pro/Max: Portable Computer is the only Perplexity path to a true local folder (install the app, enable Portable Computer, grant folder-level permission to one PT/OS folder).

**Limits that matter:** Free: ~3 Pro searches/day and ~5 Deep Research queries/day as reported (Perplexity no longer publishes exact counts, treat as approximate), limited uploads (one source cites 40 MB/file, 30-day retention). Pro: 50 files per Space, 50 MB per file (reported); Max/Enterprise Pro: 500 files; Enterprise Max: 5,000. Conflict flagged: one Oct 2026 review claims renamed Projects hold up to 10,000 files and 5 GB at 100 MB/file, conflicting with the 50-file Pro limit in Perplexity's own help-derived summaries; plan around the smaller 50-file limit until the current Projects help page is checked in the live product.

**Unverified:** exact current daily Pro Search/Deep Research counts; Free Projects availability; the 10,000-file Project claim.

**Sources:** https://www.perplexity.ai/help-center/en/articles/10672063-introduction-to-file-connectors-for-enterprise-organizations · https://www.perplexity.ai/help-center/en/articles/12870620-connecting-perplexity-with-google-drive · https://www.perplexity.ai/hub/blog/introducing-portable-computer-for-local-first-ai

---

## 10. Hermes (Nous Research model family)

**Naming warning: three different things share the Hermes name.** (a) Hermes model = the open-weight model family from Nous Research; used in a chat window, it is just a model. (b) Hermes Agent = a separate, self-hosted agent program from Nous Research, also called Hermes; this is the one with memory and files. (c) Third-party managed Hermes hosts, which package the agent with their own dashboards. Do not plan PT/OS around one and expect another's behavior.

**Plans:** Hermes Agent software itself is free, MIT licensed; you pay separately for model use and, if wanted, hosting. Nous Portal (subscription bundling model access for Hermes Agent): Free $0 (free models only, standard rate limits, $0 credits); Plus $20/mo ($22 credits, 200+ models, hosted tool use, high rate limits, $10 rollover cap); Super $100/mo ($110 credits, $50 rollover cap); Ultra $200/mo ($220 credits, $100 rollover cap). Hermes Cloud (Nous's own hosted Hermes Agent, out of preview mid-Sept 2026 per secondary coverage): Medium ~$0.56/day running (~$16.80/mo), $0.03/day stopped, 2 GB RAM, 4 vCPU; Large ~$1.09/day running, $0.03/day stopped, 4 GB RAM, 8 vCPU; compute/storage only, model/tool use billed on top; $2 minimum credits to deploy per secondary coverage. No student plan or limited student tier found for Nous Portal. Third-party managed hosts exist (e.g. Lite ~$3.99-6/mo, Pro ~$6.99-20/mo depending on host, usually with a small included AI credit); those are host prices, not Nous prices.

**1. Files across sessions?** Plain Hermes model in a chat app: no, not as a workspace; at best the app keeps chat history with an account, and each new chat is effectively a fresh start for files. Hermes Agent: yes, by design; persistent memory files (MEMORY.md, USER.md), searchable past sessions in SQLite, reusable skills as SKILL.md files, living under the Hermes home (`~/.hermes/` on macOS/Linux, `%LOCALAPPDATA%/hermes` on Windows, named profiles under `profiles/<name>/`).

**2. Local computer folder?** Plain Hermes chat: no; a browser chat cannot read the SSD, at most a per-session file upload via the browser picker, which does not become a live folder. Hermes Agent, self-installed: yes, but with a split. It runs on macOS (Apple Silicon), Windows 10/11, Linux, WSL2, or Docker, with a desktop app plus terminal, browser, and messaging surfaces. With the local backend it can work with local files; with the Docker backend, work is sandboxed, and by default the persistent workspace is bind-mounted from `~/.hermes/sandboxes/docker/<task_id>/`, not from an arbitrary folder like Documents. Reaching a specific user folder requires deliberate configuration, not just installing it.

**3. Cloud documents?** Plain Hermes chat: no native Drive/OneDrive/iCloud integration verified. Hermes Agent core: no native Drive/OneDrive/iCloud file sync verified. What exists is extensibility: MCP servers, with third-party MCP servers for Google Drive and Google Workspace configured in `~/.hermes/config.yaml` with OAuth; that is a technical setup step, not a built-in "connect Drive" button in the core product. Managed hosts may advertise Gmail/Calendar/Docs connectors, but that is host packaging.

**4. PT/OS home and simplest path, in order of simplicity:**
- A. Chat-only Hermes, simplest but weakest: PT/OS lives outside Hermes, on the user's computer or in Drive/Notes as the master copy; the carry-along form is a single short file, ideally one page, pasted or uploaded at the start of each session. Nothing persists inside Hermes between sessions.
- B. Hermes Cloud, simplest agent path: PT/OS lives in the hosted agent's workspace, with MEMORY.md and skills as the persistent layer. Setup: Portal account, subscription or credit balance, deploy a Cloud instance, chat via dashboard or Telegram/Discord/Slack/email. No terminal, VPS, Docker, or YAML editing. Tradeoff: the folder is not on the user's SSD, it is on Nous's host, model costs are extra, and secondary coverage notes Cloud gives no terminal or file browser the way a local install does, so hand-editing the folder is less direct.
- C. Self-installed Hermes Agent, most capable but not non-technical: PT/OS lives in the agent home/workspace (notes and skills under `~/.hermes/`, or a project workspace the agent is pointed at). Setup: install the desktop app or CLI, run `hermes setup --portal` or pick a provider, connect a model, optionally connect Telegram. Minutes for a comfortable user; a real barrier for a true beginner, especially with sandboxing, profiles, and provider choice.

**Limits that matter:** No official file/project/message cap found for the agent; real limits are model rate limits and API spend. A current free-tier message cap for the plain Hermes chat site could not be verified (older third-party reviews describe it as limited but appear to describe the Hermes 3 era).

**Unverified:** current file-upload/retention/message limits for the plain Hermes chat site and whether any current Nous chat product offers project folders; any Nous Portal student/education plan; Hermes Cloud's current size list and file-browser behavior from Nous's own page (daily prices above came from secondary October 2026 coverage); any native OneDrive/iCloud integration for either system.

**Sources:** https://hermes-agent.nousresearch.com/ · https://www.hermesagentai.org/ · https://openclawlaunch.com/hermes-hosting

---

## 11. OpenClaw (formerly Clawdbot, briefly Moltbot)

**Naming warning: same project, renamed after a trademark request in January 2026** per a third-party FAQ. Old guides, install URLs, and GitHub paths still use the old names.

**Plans:** OpenClaw software itself is free and open source, MIT licensed; no official paid tier and no student tier found. "Free" does not mean zero cost in practice: you still pay for a model (Anthropic or OpenAI API key on pay-as-you-go billing, a Claude Pro or similar subscription where supported, or a free local model via Ollama), a machine to run it on (your own always-on computer, or a VPS commonly cited at ~$5/mo), and optionally managed hosting sold by third parties, not by OpenClaw itself (examples found: OpenClaw Launch Lite $3 first month then $6/mo or $60/yr, Pro $20/mo or $200/yr, free 30-minute trial with no card; OpenClaw Cloud per a third-party FAQ $19/mo fully managed via Telegram/WhatsApp; other hosts ~$9.99/mo). Treat all host prices as third-party and changeable.

**1. Files across sessions?** Yes, and this is OpenClaw's core design, Tier A. Default workspace is `~/.openclaw/workspace`, configurable in setup. It holds standing files including MEMORY.md, USER.md, SOUL.md, IDENTITY.md, AGENTS.md, TOOLS.md, `memory/YYYY-MM-DD.md` daily notes, and `skills/` for reusable procedures. Sessions and transcripts are also kept in state under `~/.openclaw/`, with a searchable memory index.

**2. Local computer folder?** Yes, the strongest fit in this matrix for PT/OS, with a safety caveat. By default the main session's tools run on the host, so the agent can read and write files in its workspace and, depending on configuration, beyond it. Sandboxed sessions differ: the sandbox by default sees only `/sandbox/workspace`, and outside folders must be explicitly mounted (e.g. `mount_paths` with read-only or read-write flags). Security guides recommend the opposite of wide access: keep the agent in its own workspace, use a separate OS user or dedicated machine, block credential folders like `~/.ssh`, and do not casually symlink Documents into the workspace. No desktop app, paid plan, or self-hosting change is required to get local access; self-hosting is the normal route. With a paid managed host, files live on the host's server, not the user's SSD, unless sync/export is also set up.

**3. Cloud documents?** No built-in one-click Drive/OneDrive/iCloud sync in core OpenClaw verified. Practical bridges, with setup: the Gog skill (Google Workspace CLI skill covering Gmail, Calendar, Drive, Contacts, Sheets, Docs; install via Homebrew and ClawHub, then Google OAuth once; the agent can search Drive, export Docs, update Sheets); sync tools (sync client, rclone, or an Obsidian plugin such as Remotely Save to mirror a folder to Drive, OneDrive, Dropbox, S3, or WebDAV, then have the agent work from the local copy); third-party cloud workspaces (e.g. Fast.io MCP workspace with Cloud Import from Drive, Dropbox, OneDrive, Box, plus version history, a separate paid service, not core OpenClaw). For iCloud specifically, no direct native integration verified; the realistic route is iCloud Drive mirroring a folder to the local machine, then the agent using the local copy.

**4. PT/OS home and simplest path, and the honest technical bar:** PT/OS home, self-hosted: inside the OpenClaw workspace, e.g. `~/.openclaw/workspace/pt-os/`, or directly as the workspace's own MEMORY.md, USER.md, AGENTS.md, and `skills/` files; that is the design OpenClaw already expects. Keep a human-readable backup copy in Drive or on the computer, updated by sync or periodic export, because the workspace is otherwise tied to that one machine. Self-hosted setup in practice: (1) install Node.js 22+; (2) run the installer (e.g. `curl -fsSL https://openclaw.ai/install.sh | bash` or `npm install -g openclaw@latest`); (3) run `openclaw onboard --install-daemon` and answer the wizard (model/auth, workspace, channels, daemon for 24/7 running); (4) test first in the browser dashboard (`openclaw dashboard`, `http://127.0.0.1:18789/`) before adding Telegram/WhatsApp; (5) for Telegram create a bot with BotFather and paste the token, for WhatsApp scan a QR code with `openclaw channels login`; (6) add the Gog skill only if Drive access is actually needed. The wizard is genuinely guided, and guides claim "no programming knowledge required, just copy and paste commands." For a motivated beginner comfortable opening a terminal, that is plausible. For a truly non-technical user, it is not realistic as a solo first project; failure modes are exactly the non-technical ones (Node version problems, API key creation, Telegram bot tokens, daemon not running after reboot, Control UI security, sandbox path confusion, gateway down). The realistic non-technical path is a managed host (sign up, connect Telegram, use the host dashboard/file manager, accept PT/OS lives on the host, not the local SSD) or a technical helper doing the one-time install on an always-on Mac Mini, old laptop, or VPS, after which daily use is just messaging the agent or opening the dashboard. Bottom line: the better PT/OS home of the agent systems here, because persistence and local files are native, not bolted on, but "better home" does not mean "easy for everyone."

**Limits that matter:** No official OpenClaw file/project/message cap found. Real limits are model rate limits and API spend, plus the practical limit that a laptop agent stops when the laptop sleeps or closes. The Control UI is local by default and should not be exposed publicly without a tunnel or VPN.

**Unverified:** official managed pricing (all host prices above are third-party); a native official OneDrive or iCloud integration for OpenClaw.

**Sources:** https://openclawlaunch.com/pricing · https://agent-life.ai/openclaw_memory.html · https://clawd-bot.com/install/

---

## 12. Meta AI / Muse

**Scope note first: "Meta AI" and "Muse" are not the same product.** Meta AI is the assistant inside Facebook, Instagram, and WhatsApp. Muse is Meta's separate personal agent app (iOS, Android, web at muse.ai, WhatsApp, Mac). The PT/OS answers below are about Muse, because plain Meta AI has no persistent agent workspace. Muse launched September 2026 and its in-app connector list is still changing; the in-app list is the final authority.

**Plans:** Muse Free $0, usage-limited; Power $20/mo; Max (also called Maximum) $100/mo. Paid tiers buy weekly usage volume only, not extra features, per Meta help pages as summarized in pricing guides. Weekly allowance, reported: Free up to 100M "Muse tokens" per week, Power 500M, Max 3B (caution: the 100M free figure comes from the launch post via press reports; Meta's help page reportedly states the paid numbers but not the free number; a "Muse token" is Meta's agent-work metering unit, not a published conversion to tasks or API tokens). No file-count or project-count limit was found. No student plan found for the Muse agent (one guide states explicitly "no student-specific discount"; the free tier is the student path). Do not confuse with Meta One: Meta One Core ($7.99/mo) and Premium ($19.99/mo), launched Sept 15, 2026, buy Meta AI image/video generation and app perks, not Muse Power/Max. Availability: US from Sept 8, 2026, Canada added Sept 18, 2026, age 18+; Japan Oct 23, 2026 reported by a secondary availability tracker, not confirmed from an English Meta announcement in sources checked. A Meta account (email or phone) is enough; no Facebook account required. Recent changes: Muse for Mac launched Sept 17-18, 2026; iPad app Oct 7, 2026; Dropbox, Box, Notion, Asana, Canva and other connectors added around Sept 28-29, 2026.

**1. Files across sessions?** Yes, in Meta's cloud, but with a visibility caveat that matters for PT/OS, Tier B-. Each user gets a dedicated, isolated Linux cloud VM ("Muse Secure VM") with its own file system, terminal, browser, persistent memory, goals, side chats, background schedules, and artifacts (documents, pages, dashboards). Work survives closing the app, and Meta's technical disclosure says users can inspect and edit memory files and that VM data is continuously backed up. Caveat: this is an agent-managed workspace, not a user-browsable folder. Sources describe finished work as saved in the Muse workspace and attached to the conversation where it was made, so the user goes back to that chat or asks Muse where it put it. No source checked documents a Finder/Files-style file browser for arbitrary VM workspace files on phone or web. A PT/OS folder stored only in the VM would be real and persistent, but the non-technical user could not open, edit, or copy it directly outside Muse; they would have to ask Muse to show, edit, or download it. That makes the VM alone a weak PT/OS home for a user who wants to own and carry the files.

**2. Local computer folder?** Yes, but only on Mac, only with the Mac app, and only as opt-in, task-time access. No Windows desktop app exists. The Mac app works across local Files, Mail, Messages, Calendar, and Notes (organizing folders, completing forms from local files, summarizing messages and notes); tasks continue across phone, laptop, and WhatsApp. Local access is opt-in; macOS Full Disk Access is optional, not mandatory (guides recommend leaving it off and granting access to one folder instead). Muse settings include File System Access choices (Off, Read only, or Read and interact, per app) plus blocked folders, and sensitive actions such as deleting files or sending messages require approval. Important limit: the agent still runs in its cloud Secure VM; the Mac app bridges to local files. No source checked verifies continuous two-way sync of a folder (edit on disk, auto-reflected in Muse, and vice versa without a task running). Treat Mac local access as "Muse can read and edit files you point it at when it works on a task," not as a synced PT/OS folder.

**3. Cloud documents?** Yes for Google Drive and Dropbox; no native OneDrive or iCloud connector found. Google: in-app connector lists (Sept 14 and Oct 15, 2026) include Gmail, Google Calendar, Google Docs, Google Drive, Google Sheets, Google Slides, Google Forms, Google Tasks, Google Contacts; connector summaries describe Google Docs as read/edit and Drive as find/open; connect via Settings, then Connectors, then sign in to Google. Dropbox (clearest documented case): Dropbox's own blog (Sept 29, 2026) says Muse can search and retrieve Dropbox content and "use Dropbox tools to create and organize files and folders, create shared links, and set up file requests," with extra confirmation for changes (creating, moving, copying, deleting); available in English in the US and Canada, across all Dropbox accounts and all Muse plans including free; connect via Muse menu, Settings, Connectors, search Dropbox, Connect, sign in and authorize. Also listed: Box, Notion, Evernote, Asana, Slack, GitHub, and others in the Oct 15 in-app list. OneDrive: no OneDrive connector appears in the Sept or Oct in-app lists checked; one guide states flatly "Meta Muse has no OneDrive connector." Outlook Mail, Calendar, and Contacts connectors exist, but those are not OneDrive file storage. iCloud: no iCloud Drive connector found; indirect route only (on a Mac, files synced to iCloud Drive appear as local files, so Muse for Mac file access could reach them, but that is unconfirmed as a supported PT/OS path and should not be promised).

**4. PT/OS home and simplest path:** Best answer for a non-technical user: a Dropbox folder (or a Google Drive folder as second choice), not the Muse cloud VM and not a local folder alone. (1) Create one folder in Dropbox called PTOS (or Plain Text OS) with one short start-here file plus a small set of plain-text workflow files. Dropbox is preferred because its read/write behavior is explicitly documented by Dropbox itself and works on all Muse plans including free. (2) In Muse, go to Settings, then Connectors, search Dropbox, Connect, sign in to Dropbox. (3) In the first chat, say: "Use only my Dropbox folder PTOS as my operating system. At the start of every task, read the start-here file in that folder first, and save any updated notes back to that same folder. Ask me before deleting or moving anything." (4) Test with a tiny task ("Read my PTOS start-here file and tell me what it says"), then check in Dropbox that any file Muse created landed in the right folder. Why not the alternatives: VM workspace only is persistent but not user-browsable and locked to Muse; Mac local folder only requires a Mac, the Mac app, and careful permission scoping, and gives no access from phone or web; single carry-along file is a viable fallback for phone/web-only users (keep one master .md on their device or cloud, upload or paste it at the start of a session), but it is manual every session and edits inside Muse do not automatically update the user's copy unless Muse is told to save it back to Dropbox/Drive. Caution: do not use Muse's share-link feature for a PT/OS folder; in October 2026 researchers found about 6,800 shared Muse links discoverable via public DNS because titles were embedded in share URLs, and Meta paused conversation sharing while reviewing it. Keep PT/OS private and unshared.

**Limits that matter:** Weekly usage metering in "Muse tokens" (Free ~100M, Power 500M, Max 3B, as reported); no file/project cap found.

**Unverified:** whether the Google Drive connector can create and edit plain .txt/.md files specifically (Docs editing and Drive find/open are documented; plain-text file creation via Drive is not explicitly documented); whether Muse for Mac access is continuous sync or only task-time access (no source confirms sync); whether a phone/web user can browse the Muse VM workspace file tree directly (no source confirms a file browser); Japan availability (secondary tracker only); any post-Oct 15 connector additions.

**Sources:** https://shipwithmuse.live/blog/muse-pricing · https://blog.dropbox.com/topics/company/put-dropbox-project-context-to-work-meta-muse · https://www.kdnuggets.com/meta-muse-explained-what-it-is-how-it-works-and-what-it-can-do

---

## 13. DeepSeek (Hangzhou, China)

**Plans:** Free $0 consumer chat at chat.deepseek.com and in mobile apps; no ads and no in-app purchases per the company's January 2025 app announcement. The developer API is paid per token and is separate from chat. No projects feature found; no student plan found.

**1. Files across sessions?** Tier C, paste-in plus uploads. Conversation history with memory inside a thread; file upload (PDF, Word, Excel, images) and long-context conversations reported. One secondary source claims up to 1M tokens of context, another describes 128K, so do not quote an exact context number. No persistent project or library container found: the PT/OS home is the carry-along file pasted into a thread, with the master copy kept outside. The user re-pastes after changes.

**2. Local computer folder?** No. Web and app chat only; no SSD access.

**3. Cloud documents?** No Drive or OneDrive connector found for consumer chat. Uploads are per-conversation.

**4. PT/OS home and simplest path:** Single carry-along file, pasted into a DeepSeek thread. Same pattern as Duck.ai: paste the file, work, ask for the full updated file after each task ("checkpoint"), save it over the master copy. Conversation history inside the thread is a backup of last resort, not the master copy.

**Privacy note that matters for PT/OS users:** secondary sources report chats are stored on servers in China. PT/OS's generic privacy guidance applies: check the service's privacy settings and decide what you are comfortable sharing. Do not present DeepSeek as a privacy-first option.

**Unverified:** exact context limit; whether thread memory persists across long gaps; file upload size limits on free chat.

**Sources:** search-verified Oct 27, 2026 (not guinea-pig tested).

---

## 14. Lumo (Proton, Switzerland)

**Plans:** Free $0, no account required to start chatting at lumo.proton.me; a free Proton account adds encrypted saved history and more messages. Free limits: limited messages and chat history, small file uploads, one Project. Plus $12.99/mo monthly ($9.99/mo annual): unlimited chats, extended history, unlimited Projects, multiple large file uploads. No student plan found.

**1. Files across sessions?** Tier B on free (one Project) and fuller Tier B on Plus. Projects group chats and files; free tier includes one Project, small file uploads, web search, and basic chat history with a free Proton account. Zero-access encryption on chats: Proton states it cannot read conversations, chats are not logged, and data is not used for training. Proton Drive integration exists (limited on free, fuller on Plus).

**2. Local computer folder?** No. Web and app chat only; no SSD access.

**3. Cloud documents?** Proton Drive linking reported (limited on free). In-place .md editing in Drive via Lumo not verified; treat as upload/replace pattern until tested.

**4. PT/OS home and simplest path:** Free: one Project called PT/OS holding the carry-along file plus any workflows, with the master copy kept outside (a folder or Proton Drive). Signed-out use is paste-in only, since there is no saved history without an account. Plus: unlimited Projects, same pattern at larger scale. Lumo is the strongest privacy-first PT/OS home in this matrix and a natural fit for users who already use Proton Mail or Drive.

**Unverified:** exact free message caps (Proton does not publish them); whether a Project's files can be edited in place; Drive sync behavior.

**Sources:** search-verified Oct 27, 2026 (not guinea-pig tested).

---

## 15. Qwen (Alibaba, China)

**Plans:** Free $0 consumer chat at chat.qwen.ai and in mobile apps. Basic use reported without an account; sign-in saves chat history and raises usage limits. Open-weight models (Qwen2.5, Qwen3) are also freely downloadable for developers to self-host, but that is not the consumer PT/OS path. No subscription required for chat; no student plan found.

**1. Files across sessions?** Tier C, paste-in plus uploads. Conversation history with an account; file upload (CSV, Excel, text, PDF, images) and long-context file analysis reported, with Qwen claiming up to 1M tokens for file processing (vendor claim, not independently confirmed). No persistent project or library container found: the PT/OS home is the carry-along file pasted into a thread, with the master copy kept outside. Strong multilingual support (100+ languages reported), which matters for PT/OS's planned German, Spanish, and Romanian translations.

**2. Local computer folder?** No. Web and app chat only; no SSD access.

**3. Cloud documents?** No Drive or OneDrive connector found for consumer chat. Uploads are per-conversation.

**4. PT/OS home and simplest path:** Single carry-along file, pasted into a Qwen thread. Same pattern as Duck.ai and DeepSeek: paste the file, work, ask for the full updated file after each task ("checkpoint"), save it over the master copy. With an account, thread history is a backup of last resort, not the master copy.

**Privacy note that matters for PT/OS users:** one review reports Qwen's default terms let stripped-down chats help train the models. PT/OS's generic privacy guidance applies: check the service's privacy settings and decide what you are comfortable sharing. Do not present Qwen as a privacy-first option.

**Unverified:** exact context limit; exact free usage caps; whether basic no-account use persists across sessions.

**Sources:** search-verified Oct 27, 2026 (not guinea-pig tested).

---

## Cross-system summary: the PT/OS home on each system

| System | Tier | Best PT/OS home for a non-technical user | Free tier usable for PT/OS? |
|---|---|---|---|
| ChatGPT | B (A on desktop) | Project + one carry-along file; Drive folder via Work; local folder via desktop Work (Plus) | Yes, with 5-file Project cap |
| Claude | B (A on desktop, paid) | Project + one carry-along file; Drive folder via connector; local folder via Cowork (Pro, cloud-default since Oct 6, 2026) | Yes, with 5-project cap |
| Gemini | B | Drive folder + one master Doc + Gem/Notebook pointer; Spark local folders Mac-only, paid | Yes, with 10-file Gem limit |
| Grok chatbot | B/C | Project + carry-along file; private GitHub repo via Connectors as portable option | Carry-along yes; Projects on Free unconfirmed |
| Grok Bot | A (cloud computer) | Bot's persistent cloud workspace (`/workspace` per secondary sources) | No, Premium $30/mo+ |
| Copilot | B | OneDrive folder + Notebook pointer; free = upload-each-session only | Weak; upload-each-time only |
| Mistral Vibe | B | Project + Library in Vibe; master copy kept outside, re-uploaded | Yes |
| Brave Leo | C+ | Folder on the user's computer; paste START HERE each session; optional local Memories | Yes, device-only |
| Duck.ai | C | Master folder outside; paste 1-page START HERE every session; copy revisions back by hand | Yes, paste-only |
| Perplexity | B | Project + one master file + Drive backup, re-imported after edits; Portable Computer only on paid + qualifying hardware | No, do not build on Free |
| Hermes chat | C | Master file outside; re-pasted single file every session | Yes, paste-only |
| Hermes Agent | A | Agent workspace (`~/.hermes/` or hosted Cloud workspace) | Agent software free; model/hosting costs apply |
| OpenClaw | A | Workspace (`~/.openclaw/workspace/`) as master, Drive copy as backup; managed host for non-technical users | Software free; model/machine costs apply |
| Meta Muse | B | Dropbox folder (best documented) or Drive folder via Connectors; VM workspace alone is not user-browsable | Yes, including Dropbox on free |
| DeepSeek | C | Single carry-along file pasted into a thread; master copy outside | Yes, free chat |
| Lumo | B (free: 1 Project) | One Project holding the carry-along file; master copy outside or in Proton Drive | Yes, including no-account chat |
| Qwen | C | Single carry-along file pasted into a thread; master copy outside | Yes, free chat; account saves history |

## Design takeaways for PT/OS

1. **The 1-page carry-along file is the only universal format.** It works on every system in this matrix, including Duck.ai, Leo, and free Grok, where it is the ONLY format that works. Every per-system guide should start from it.
2. **Projects/Libraries/Gems/Notebooks are the portable Tier B home** on ChatGPT, Claude, Gemini, Mistral, Grok, Perplexity, and Lumo, but in every case the in-app copy is a snapshot: the user must re-upload or re-import after edits. No system in this set was verified to auto-sync a disk folder into its Project container.
3. **True local-folder (Tier A) access always requires a desktop app and usually a paid plan:** ChatGPT Work/Codex desktop, Claude Cowork desktop (Pro+, cloud-default since Oct 6, 2026), Gemini Spark Mac-only, Perplexity Portable Computer (paid + qualifying hardware only), Hermes Agent, OpenClaw, Muse for Mac only. Web/mobile chat alone never touches the SSD on any system.
4. **Cloud-doc homes differ by vendor ecosystem:** Drive for Gemini/ChatGPT/Claude/Muse, OneDrive for Copilot, Dropbox for Muse (best documented), GitHub for Grok. No system verified a native iCloud Drive connector; the iCloud route everywhere is a locally synced folder used by a desktop agent.
5. **In-place editing of a plain .md file is the weakest-verified capability in the whole matrix.** It is solid only in Tier A local folders and agent workspaces. In Drive/OneDrive/Project containers, the verified pattern is create-new, export, or replace/re-upload, not silent in-place rewriting of the same .md. PT/OS guides must not promise it where it is unverified.
6. **Student plans worth noting:** Mistral Student $5.99/mo (Pro features); Perplexity Education Pro $10/mo; Gemini AI Pro free 12 months for eligible US students (Plus free 12 months in 140+ other markets, redeem by Dec 31, 2026). No student plan found for Claude, Grok, Copilot (current), Leo, Duck.ai, Hermes Portal, OpenClaw, or Muse. ChatGPT's student offer was time-limited (4 free months of Plus, claim by Oct 31, 2026).
7. **Two naming traps to warn users about in the guides:** Hermes = model vs Hermes Agent vs third-party hosts; OpenClaw = formerly Clawdbot/Moltbot; Mistral Le Chat = now Vibe (May 28, 2026); Grok chatbot vs Grok Bot; Meta AI vs Muse.
