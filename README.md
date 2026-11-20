# Airsurf for Claude Code

[Airsurf](https://airsurf.app) is one workspace for a team's docs, issues, projects, calendar and designs, linked so a
change shows everywhere. This plugin gives Claude Code the same context as every other AI tool you connect to Airsurf:

- **MCP server** `https://airsurf.app/api/v1/eco/mcp` — search, read, create and link docs, issues, projects and
  events; branch names and pull-request links for issues. Sign-in is OAuth in your browser; Claude Code only gets what
  your Airsurf account may see, and every change can be undone.
- **Skill `airsurf-context`** — before working on an issue, Claude reads its brief, decisions and linked work.
- **Skill `save-to-airsurf`** — at the end, Claude saves what was decided as a page, issues or a comment.

## Install

    /plugin marketplace add hskzl/airsurf-claude-plugin
    /plugin install airsurf@airsurf

Then run `/mcp`, choose **airsurf** and sign in. Without the plugin, the server alone:

    claude mcp add --transport http airsurf https://airsurf.app/api/v1/eco/mcp

## Links

- Docs: https://airsurf.app/developers/ecosystem#mcp
- Privacy: https://airsurf.app/legal/privacy
- Support: https://airsurf.app/support
