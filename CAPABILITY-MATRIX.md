# PT/OS Capability Matrix

**PT/OS Workspace: Can this AI maintain files that you own?**

Reviewed: October 28, 2026. This document replaces the earlier single-file-first recommendations. It focuses on whether an AI can read, create, and update files in persistent storage. Product features change quickly, so verify capabilities in the account and environment being used.

The matrix is technical reference material for `AGENT.md` and for anyone comparing platforms. The user does not need to read it to begin setup.

## What Qualifies for Workspace?

PT/OS Workspace requires all of the following:

1. **Read:** The AI can open the current files in the selected location.
2. **Create:** The AI can create a new file or supported document there.
3. **Update:** The AI can edit an existing file without requiring the person to copy and replace its contents manually.
4. **Persist:** The files remain available after the conversation ends.
5. **Verify:** The AI can confirm that its changes were saved to the intended location.
6. **Export:** The person can retrieve or export the files independently of the AI service.

These are requirements of the *configured tools*, not properties of a model name. A chat assistant, desktop agent, cloud agent, and connected app can behave differently even when they use the same model.

**Do not count uploaded reference files or chat history as writable storage.** A Project, Library, Gem, Notebook, or similar collection may remember uploaded documents but still leave the user responsible for replacing them. That is not sufficient for PT/OS Workspace.

### Classification

- **Documented route:** Vendor documentation identifies a plausible persistent read/write path. The setup must still pass the Workspace file test.
- **Conditional route:** A capable product or connector may support Workspace, but the required editing and persistence have not been established for the specific configuration. Test before recommending.
- **PT/OS One route:** Ordinary chat or uploaded-file access does not provide reliable persistent write-back. Use the separate single-document product.

No classification guarantees that a particular account, plan, permission set, or device will work.

### Mandatory File Test

Before creating a workspace, ask approval to use an intended storage location. Create a small test file, read it back, edit that same file, and read the revision back. Confirm that it is saved in persistent storage the person can access. If the test fails, explain the missing capability and stop Workspace setup. Never infer write access from a connector's ability to search or summarize files.

## Platform Summary

| AI / Configuration | Workspace assessment | Viable storage route or limitation |
|---|---|---|
| **ChatGPT with file-writing tools** | Documented route | GitHub write access; desktop Work/Codex local folder; authorized Google Docs/Drive edits |
| ChatGPT Projects with uploaded files only | PT/OS One route | Project knowledge is not proof of in-place file editing |
| **Claude Cowork / Claude Code** | Documented route | Approved local folders; Google Docs edits when the required connectors are enabled |
| Claude chat Projects with uploads only | PT/OS One route | Persistent references do not establish writable source files |
| **Gemini with an authorized editing tool** | Conditional route | Verify actual create/edit access in Google Drive or a local agent environment |
| **Grok with GitHub write tools / Grok Bot** | Conditional route | Verify the specific connector or cloud workspace can edit and retain files |
| **Microsoft Copilot Cowork** | Documented, restricted route | Supported Office documents in OneDrive or SharePoint; confirm account and permissions |
| Consumer Copilot chat without write tools | PT/OS One route | Chat or cloud-file search alone is insufficient |
| **Mistral Vibe Code** | Conditional route | A configured local coding workspace may supply read/write access |
| Mistral chat Projects/Libraries | PT/OS One route | Persistent uploads are not verified source-file editing |
| Brave Leo | PT/OS One route | No verified persistent file write-back |
| Duck.ai | PT/OS One route | Paste or upload documents; no verified persistent file write-back |
| **Perplexity Portable Computer** | Conditional route | Qualifying local setup with confirmed read/write permissions |
| Perplexity Projects / Drive connector | PT/OS One route | Imported files are snapshots; the Drive connector does not edit source content |
| **Hermes Agent (local or hosted)** | Documented route | Persistent agent workspace; verify access and export on hosted installations |
| Hermes model in ordinary chat | PT/OS One route | The model itself supplies no persistent filesystem |
| **OpenClaw** | Documented route | Local or hosted agent workspace, with restricted permissions |
| **Muse with a writable connected folder** | Conditional route | Check file-content updates in Dropbox, Drive, or approved local files |
| DeepSeek consumer chat | PT/OS One route | No verified persistent file write-back |
| Lumo consumer chat / Projects | PT/OS One route | Proton Drive access does not establish in-place editing |
| Qwen consumer chat | PT/OS One route | No verified persistent file write-back |

## Platform Notes

### 1. ChatGPT (OpenAI)

**Workspace route:** Use ChatGPT with verified GitHub write permissions, Work or Codex with an approved local folder, or a connected Google Drive account with supported create/edit actions. Google Docs, Sheets, and Slides can be edited in place where the action is enabled and authorized. ChatGPT Projects can hold persistent context, but uploaded Project files alone are not a writable folder.

**Checks:** Confirm the actual mode, plan, connector permissions, destination, and write operation. Local files require the relevant desktop environment; cloud access does not imply access to a user's computer. A Google Docs-based workspace may be practical, but exportable copies are important when moving to another AI.

Sources: [OpenAI Work file editing](https://help.openai.com/en/articles/20001278-creating-and-editing-documents-spreadsheets-and-presentations-with-chatgpt-work) · [Google Drive setup](https://help.openai.com/en/articles/10929079-google-drive-app-and-setup-in-chatgpt) · [Work and Codex](https://help.openai.com/en/articles/20001275-chatgpt-work-and-codex)

### 2. Claude (Anthropic)

**Workspace route:** Claude Cowork can read and write approved local folders when the Claude Desktop app provides access. Claude Code can work directly with files in an authorized project directory. Claude can also edit native Google Docs, Sheets, and Slides using the relevant connectors; an ordinary Google Drive search connection is not the same as authorization to edit.

**Checks:** For local files, the desktop app must remain available while cloud sessions access the folder. Claude Projects and their uploaded knowledge files are not automatically updated by Cowork. Test the intended source document rather than assuming Project context is the master copy.

Sources: [Cowork across devices](https://support.claude.com/en/articles/15520349-use-claude-cowork-on-web-desktop-and-mobile) · [Google Workspace connectors](https://support.claude.com/en/articles/10166901-use-google-workspace-connectors)

### 3. Google Gemini

**Workspace route:** Google Drive is the natural candidate, and some Gemini surfaces can work with documents there. A developer-focused local environment, such as Antigravity, may also provide file tools. The former matrix's recommendation to place one master document inside a Gem or Notebook is insufficient for Workspace unless the AI can edit that persistent master directly.

**Checks:** Verify both creation and repeat editing of the selected documents in the actual Gemini product. Do not assume that being able to reference a Drive document, save a new document, or update content inside a document editor also authorizes maintenance of an entire Drive folder. Plan, device, and surface restrictions require live verification.

Reference: [Google's Gemini documentation and help](https://support.google.com/gemini/)

### 4. Grok (xAI)

**Workspace route:** A GitHub integration with confirmed commit/write tools could support a private repository. A persistent Grok Bot environment may also qualify if the person can access and export its files. The ordinary chatbot's Projects or uploaded files do not qualify by themselves.

**Checks:** Connector availability does not prove file-write scope. Verify repository permissions and read-back after a commit, or confirm that a Bot's workspace persists and remains independently exportable. Grok chatbot and Grok Bot should be evaluated separately.

Reference: [Grok connectors](https://docs.x.ai/grok/connectors)

### 5. Microsoft Copilot

**Workspace route:** Microsoft Copilot Cowork can edit supported Office documents stored in OneDrive or SharePoint, saving changes to the same file. This provides a credible document-based Workspace route for accounts with Cowork access and the required permissions. It does not establish that every consumer Copilot chat can maintain a folder of Markdown files.

**Checks:** Verify licensing, accessible cloud location, supported document formats, and the edit action. Cowork cannot directly read or edit local device files; a locally synced OneDrive copy does not change that limit. Consumer chat and Cowork must be treated as different configurations.

Sources: [Use Copilot Cowork](https://learn.microsoft.com/en-us/copilot/cowork/use-cowork) · [Cowork limitations](https://learn.microsoft.com/en-us/microsoft-365/copilot/responsible-ai/copilot-cowork-application-card)

### 6. Mistral (Vibe)

**Workspace route:** Vibe Code may support a local project directory through coding tools. The normal chat experience, Projects, Libraries, and generated Canvas outputs have not been verified as an automatic edit-in-place system for external source files.

**Checks:** Confirm local filesystem permissions and the same-file update cycle before setup. Creating a document and downloading it does not qualify as maintaining the original. Technical setup requirements should be explained rather than presented as a beginner default.

Reference: [Mistral Vibe Code documentation](https://docs.mistral.ai/vibe/code/overview)

### 7. Brave Leo

**Workspace route:** No verified persistent source-file editing in ordinary Leo chat. Device-local chat history, memories, pasted text, or attached PDFs can carry context, but they do not let Leo maintain a user-controlled file collection.

**Recommendation:** Use PT/OS One unless another authorized tool supplies persistent read/write access.

Sources: [Brave Leo](https://brave.com/leo/) · [Leo Memories](https://brave.com/whats-new/leo-memories/)

### 8. DuckDuckGo Duck.ai

**Workspace route:** No verified file-writing connector or persistent agent workspace. Duck.ai can be used with pasted text or uploaded documents, but the person must keep and replace the master document outside the chat.

**File limits:** User testing found that a 10-page, approximately 7 MB PDF was rejected with a 5 MB limit. A 15-page PDF ceiling was separately reported during PT/OS research; it was not established by that 10-page test. Treat the page and file-size limits as independent, check the current upload interface, and do not promise a universal token limit.

**Recommendation:** PT/OS One. There is no Workspace route in ordinary Duck.ai chat.

Reference: [Duck.ai privacy and chat help](https://duckduckgo.com/duckduckgo-help-pages/duckai/ai-chat-privacy)

### 9. Perplexity

**Workspace route:** Portable Computer may provide local read/write access on supported devices and plans. Verify that the available tool can edit persistent files and that the person can retrieve them. Standard Projects and uploaded files are not a substitute.

**Important distinction:** Perplexity's Google Drive connector can search source files and import copies into Projects, but Perplexity states that it does not modify Drive file contents. Imported Project files must be imported again to reflect external edits. A read-enabled Drive connector therefore fails Workspace's write requirement.

Sources: [Perplexity Google Drive connector](https://www.perplexity.ai/help-center/en/articles/12870620-connecting-perplexity-with-google-drive) · [Portable Computer](https://www.perplexity.ai/hub/blog/introducing-portable-computer-for-local-first-ai)

### 10. Hermes (Nous Research)

**Workspace route:** Hermes Agent provides persistent files and memory in a local or hosted agent environment. It is a plausible Workspace home when the agent can edit files, retain them between sessions, and make them available for export. The Hermes model running in an ordinary chat window does not provide those features by itself.

**Checks:** Separate the model, the agent software, and any third-party managed hosting service. Local, containerized, and hosted installations have different filesystem boundaries. Verify the actual workspace path, permissions, persistence, and backup method.

Reference: [Hermes Agent](https://hermes-agent.nousresearch.com/)

### 11. OpenClaw

**Workspace route:** OpenClaw maintains a persistent agent workspace with files used for memory, instructions, and skills. It is a natural fit for a multi-file PT/OS Workspace. An authorized folder inside that workspace is sufficient; wider access to the computer is not needed.

**Checks:** Restrict tool permissions, protect credentials, and verify that the person can export and back up the workspace. Self-hosted and managed installations store files in different locations. Installation and model costs are separate from the PT/OS project.

Reference: [OpenClaw documentation](https://docs.openclaw.ai/)

### 12. Muse

**Workspace route:** Connected cloud storage or an authorized local folder may support Workspace when the available Muse tools can both read and update existing file contents. Access to a persistent agent VM or the ability to create folders is not enough to confirm a usable, portable master copy.

**Checks:** Test the actual connector, including editing an existing file and reading it back. Confirm where the files live, whether the person can browse or export them independently, and whether the connector works on the chosen device. Prior research favored Dropbox as a candidate, but reliable same-file content edits still require verification.

References: Consult the current in-app connector descriptions and permission prompts. Earlier third-party feature reports are not sufficient proof of write-back.

### 13. DeepSeek

**Workspace route:** No verified persistent read/write storage in consumer chat. Uploads and thread history can help with context, but they do not maintain a user-controlled collection of files.

**Recommendation:** PT/OS One. Reassess only if the person uses an external tool or agent environment that independently meets the Workspace test.

Reference: [DeepSeek](https://www.deepseek.com/)

### 14. Lumo (Proton)

**Workspace route:** Lumo Projects and Proton Drive access can help users work with stored information, but this matrix has not verified repeated direct edits to the same user-controlled source file. Privacy-oriented storage alone does not meet the Workspace read/write requirement.

**Recommendation:** PT/OS One for ordinary Lumo chat. Reclassify only after a supported connector or tool passes the persistent file test.

Reference: [Lumo](https://lumo.proton.me/)

### 15. Qwen

**Workspace route:** No verified persistent source-file writing from the ordinary consumer chat interface. File uploads and conversation history are not a managed folder.

**Recommendation:** PT/OS One for ordinary chat. A separate developer agent with verified filesystem access should be evaluated as that agent environment, not assumed to be a feature of Qwen chat.

Reference: [Qwen](https://chat.qwen.ai/)

## Format and Portability Rules

Workspace prefers plain-text files, including `.md` and `.txt`, because they are easy to inspect, back up, and transfer. Native Google Docs and Microsoft Office documents are valid when the AI can edit them reliably and the person can export their contents.

A document in a cloud service is not automatically available to every AI. When changing providers, check access permissions, document formats, embedded links, and dependent connectors. Keep `START-HERE.md`, or an equivalent entry document, self-contained so another AI can understand the workspace without retrieving the original PT/OS repository.

For a Workspace transfer, verify the destination's read/write tools before moving the master files. Preserve the originals until the person confirms that the new copy works.

## Guidance for AI Assistants

1. Follow `AGENT.md` for setup, approval, maintenance, and security behavior.
2. Treat this matrix as a starting point. Verify current tools, permissions, and supported actions in the actual environment.
3. Choose a storage location only after confirming the person can access and export its contents.
4. Run the create → read → update → read-back test before describing a configuration as Workspace-compatible.
5. Do not recommend manual re-upload or copy-and-paste as a Workspace solution. That is the purpose of PT/OS One.
6. Do not buy a subscription, connect a service, publish content, or enable broad filesystem access without the person's approval.
7. State what is unverified. A vendor feature description is not a completed end-to-end test.

## Research Notes

The previous matrix, researched October 27, 2026, mixed persistent reference containers with editable file systems and included numerous volatile prices, message quotas, launch dates, and third-party feature reports. Those details are intentionally excluded here because they do not establish Workspace suitability and become outdated quickly.

Vendor documentation was checked for the most consequential write-access distinctions on October 28, 2026. Other classifications inherit cautious assessments from earlier research and are explicitly conditional where the required edit cycle has not been established. No end-to-end account tests were performed as part of this revision. The Duck.ai 5 MB observation comes from the user's reported hands-on test.

Update this matrix when an actual tool test or current vendor documentation changes a platform's Workspace eligibility. Prioritize file behavior over plan marketing, and record the configuration tested rather than declaring a whole AI brand compatible.
