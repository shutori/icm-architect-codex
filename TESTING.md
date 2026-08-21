# Test ICM Architect for Codex locally

Use a local marketplace while this repository remains private. Codex’s official plugin workflow is: review the manifest and bundled skills, refresh Codex, install from a local marketplace, and test in a new task.

## 1. Clone this repository to a permanent local folder

```powershell
git clone https://github.com/shutori/icm-architect-codex.git "$env:USERPROFILE\plugins\icm-architect-codex"
```

Use a folder you will keep; a local marketplace points to files on your machine.

## 2. Add the existing plugin to your personal marketplace

In a new Codex task, invoke `$plugin-creator` and say:

> Add the existing plugin at `C:\Users\<your-user>\plugins\icm-architect-codex` to my personal local marketplace. Do not modify or scaffold over its files.

The plugin creator will create or update the personal marketplace entry and return the correct install action for your environment.

## 3. Install and refresh

Refresh the Codex desktop app, open the Plugins area, and install **ICM Architect for Codex** from your personal marketplace. Then start a **new task**; a new task is the clean boundary for Codex to load the newly installed skill.

## 4. Try representative prompts

Use one prompt at a time:

- `ICM this: every Friday I turn a list of links into a researched, reviewed newsletter.`
- `Structure this for Codex agents: I create a client brief from call notes, research, and a final approval.`
- `Map this repo so later agents can safely change it.`
- `Audit this folder and propose an ICM restructure; do not move anything before I approve the map.`

## Expected behavior

The skill should choose Build or Restructure mode, ask only the information needed to identify the repeating unit and approval gates, select the smallest ICM form, and present a proposed tree before creating or moving workspace files. Generated workspaces should use `AGENTS.md` as their one routing entry point and include explicit `CONTEXT.md` contracts. For restructure requests, it must inventory and present a migration map before making any change.

## Update after a change

Keep your local clone current, then ask `$plugin-creator` to update the already-installed plugin from that same local marketplace. It will refresh the Codex cachebuster and return the correct reinstall action. Start another new task after reinstalling.
