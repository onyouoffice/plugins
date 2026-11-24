# Onyou Office plugin

Onyou Office is a free, open-source desktop office suite. This plugin teaches
Claude Code and Codex to create, convert, read and edit real Office files on
your computer through Onyou Office's `onyouoffice` command: slide decks,
spreadsheets, Word and Hangul (HWP) documents, PDFs, draw.io diagrams and mind
maps.

## Requirements

Install the Onyou Office desktop app from
[onyouoffice.com](https://onyouoffice.com/en/download/) (Windows, macOS beta,
Linux beta). The app provides the `onyouoffice` command; the plugin contains
only the agent skill that describes how to use it. If the command is not on
the PATH yet, open the app once and use **Settings → Integrations**.

## Install

```bash
# Claude Code
/plugin marketplace add onyouoffice/plugins
/plugin install onyouoffice@onyouoffice

# Codex
codex plugin marketplace add onyouoffice/plugins
codex plugin add onyouoffice
```

## What it runs and sends

The skill tells the agent to run the `onyouoffice` command on files you point
it to. Documents are read and written on your computer. A few commands send
data off the machine, and only when the agent uses them: `search`, `image`,
`media`, `pdf ai-read`, `pdf translate` and `epub translate` send their input to
the AI provider you configured in Onyou Office, and `read-url` fetches the
address it is given. The plugin itself has no hooks, no MCP server and no
network access. To add Onyou Office as an MCP server, run
`onyouoffice mcp install claude-code` (or `codex`).

## Example requests

- "Turn these meeting notes into a 6-slide presentation."
- "Convert this PDF into an editable Word document."
- "Build a budget spreadsheet from this CSV with totals."

## Links

- Website: <https://onyouoffice.com>
- Privacy: <https://onyouoffice.com/en/privacy/>
- Source and issues: <https://github.com/onyouoffice/onyouoffice>
- Support: support@onyouoffice.com

Licensed under Apache-2.0.
