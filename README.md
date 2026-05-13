# agent-vdesktop-skill

A Claude Code **skill** plugin teaching Claude how to drive the [`agent-vdesktop`](https://github.com/Seretos/agent-vdesktop) MCP server (Windows Virtual Desktop orchestration, layouts, app launchers).

This plugin ships **only the skill content** — no binaries, no MCP server.

## Requires

This plugin formally declares `agent-vdesktop` as a dependency in `.claude-plugin/plugin.json`. Claude Code will install/load it automatically when this plugin is installed. Without `agent-vdesktop`, the tools the skill describes (`create_desktop`, `apply_layout`, `launch_*`, …) are not available.

## Install

```
/plugin marketplace add Seretos/agent-marketplace
/plugin install agent-vdesktop@agent-marketplace          # the MCP server (required)
/plugin install agent-vdesktop-skill@agent-marketplace    # this skill
```

## What the skill teaches

See `skills/vdesktop/SKILL.md` for the full mental model — desktops as containers, layouts as named slots, launchers that pin to slots, multi-monitor handling.
