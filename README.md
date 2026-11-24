# claude-better-sessions

A pane next to the Claude Code chat that shows your sessions by project: the ones where Claude is working, the ones with an open PR, the ones touched in the last 24 hours. Click a session to open it.

The plugin is named **Chantiers** (French for "work sites"), which is the label you will see in the app.

## What you see

- One card per project. The project comes from your sidebar sections, or else from the folder name.
- One dot per session: green when Claude is working, yellow for an open PR, blue for recent activity, grey for an idle session.
- Idle sessions are hidden. A button at the bottom of the pane shows them.
- A bar above the prompt input, with the **▤ Chantiers** button to open or close the pane. The `/chantiers` command does the same.
- The list refreshes on its own every 15 seconds.

## Requirements

The Claude Code desktop app on macOS. The pane reads the session list with a tool specific to the app and opens a session with the macOS `open` command. In the terminal or on Windows, it shows « Lecture impossible » (unable to read).

## Installation

From a terminal:

```bash
claude plugin install chantiers --marketplace ChristopheHvd/claude-better-sessions
```

In a Claude Code session started from a terminal:

```
/plugin install chantiers --marketplace ChristopheHvd/claude-better-sessions
```

In the desktop app, where `/plugin` does not work: click **+** next to the prompt input, then **Plugins**, **Add marketplace** with `ChristopheHvd/claude-better-sessions`, then **Add plugin**.

The pane appears in new sessions.

## Uninstall

```bash
claude plugin uninstall chantiers
```
