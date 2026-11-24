# Onyou Office plugins

Plugins that let Claude Code and Codex create, convert, read and edit Word,
Excel, PowerPoint, PDF and Hangul (HWP) documents on your computer with
[Onyou Office](https://onyouoffice.com), a free, open-source desktop office
suite.

| Plugin                                | What it adds                                            |
| ------------------------------------- | ------------------------------------------------------- |
| [`onyouoffice`](plugins/onyouoffice/) | The `onyouoffice` agent skill (no hooks, no MCP server) |

## Install

Install the Onyou Office desktop app first:
<https://onyouoffice.com/en/download/>. The plugin teaches the agent to use
the `onyouoffice` command that the app provides.

```bash
# Claude Code
/plugin marketplace add onyouoffice/plugins
/plugin install onyouoffice@onyouoffice

# Codex
codex plugin marketplace add onyouoffice/plugins
codex plugin add onyouoffice
```

## Source

The skill is maintained in
[onyouoffice/onyouoffice](https://github.com/onyouoffice/onyouoffice) under
`skills/onyouoffice/SKILL.md` and copied here when its version changes.
Report problems there or at support@onyouoffice.com.

Licensed under Apache-2.0. See [LICENSE](LICENSE) and [NOTICE](NOTICE).
