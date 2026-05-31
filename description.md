# agent-vdesktop-skill

Teaches Claude Code how to drive the `agent-vdesktop` MCP server —
Windows Virtual Desktop orchestration, window layouts, and app launchers.

## Key features

- Create, rename, switch, and delete Windows Virtual Desktops by name or index
- Apply window layouts to desktops: built-in presets (two-columns, grid-2x2,
  main-sidebar, …) or custom percent splits (columns, rows, grid, freeform regions)
- Multi-monitor layout support — assign layouts per physical screen, slots
  auto-suffixed to avoid collisions
- Launch Chrome (tabs), Windows Terminal (multi-tab, WSL or PowerShell),
  VS Code (folder/files), and arbitrary executables directly into named layout slots
- Address previously launched windows by label across turns — no re-querying
- Pin windows or entire apps across all desktops (Windows 11 native feature)
- Adopt existing unmanaged windows into the registry after a server restart
- Find windows by title or Chrome tab by URL/title
- Works whether Claude Code runs natively on Windows or inside WSL
