# Install ICM Architect for Codex

## 1. Clone the repository

Choose a permanent local folder. Codex loads local plugins from files on your machine.

```powershell
git clone https://github.com/shutori/icm-architect-codex.git "$env:USERPROFILE\plugins\icm-architect-codex"
```

## 2. Add it to your personal marketplace

In a new Codex task, invoke `$plugin-creator` and say:

> Add the existing plugin at `C:\Users\<your-user>\plugins\icm-architect-codex` to my personal local marketplace. Do not modify or scaffold over its files.

The plugin creator will register the local source and provide the correct install action for your Codex environment.

## 3. Install the plugin

Refresh the Codex desktop app, open the Plugins area, and install **ICM Architect for Codex** from your personal marketplace.

Start a new Codex task after installation so Codex can load the `icm-architect` skill.

## 4. Use it

Ask Codex to:

- `ICM this: every Friday I turn a list of links into a researched, reviewed newsletter.`
- `Structure this for Codex agents: I create a client brief from call notes, research, and a final approval.`
- `Map this repo so later agents can safely change it.`
- `Audit this folder and propose an ICM restructure; do not move anything before I approve the map.`

The skill chooses Build or Restructure mode, proposes the workspace before creating or moving files, and uses `AGENTS.md` as the routing entry point in generated workspaces.

## Update the plugin

Pull the newest changes in your local clone, then ask `$plugin-creator` to update the already-installed plugin from the same local marketplace. Start a new Codex task after reinstalling.
