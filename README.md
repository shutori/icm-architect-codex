# ICM Architect for Codex

An unofficial Codex compatibility adaptation of [RinDig/icm-architect](https://github.com/RinDig/icm-architect).

This plugin brings the Interpretable Context Methodology (ICM) to Codex: a way to structure repeatable workflows, knowledge, and editable systems as small, navigable Markdown workspaces. Folder sequencing carries order, hierarchy scopes context, and files hold visible state.

The original method and skill were created by RinDig and are used here under the upstream MIT license. This repository is a narrow patch for Codex—not a replacement for, or an independent reinvention of, the upstream project. The compatibility changes use `AGENTS.md` as the one generated routing entry point and clarify that Codex instructions and approval rules remain authoritative.

## Install

Install this repository as a local Codex plugin, then enable **ICM Architect for Codex**. The plugin exposes the `icm-architect` skill.

## Use

Ask Codex to:

- “ICM this workflow”
- “Structure this for Codex agents”
- “Make a prompt workspace for weekly reports”
- “Map this repo so later agents can safely change it”
- “Audit this folder and propose an ICM restructure”

The skill selects the smallest suitable ICM form, proposes the workspace before changing it, and uses the walk test to make sure a cold agent can navigate from `AGENTS.md` and its contracts alone.

## What is included

- Build and Restructure modes
- Six ICM forms: Pipeline, Umbrella, Record library, Knowledge bundle, Context map, and System map
- Markdown templates for routing, contracts, records, processes, schemas, and setup
- The original ICM references, adapted only where Codex routing requires `AGENTS.md`

## Credit and license

Upstream: [RinDig/icm-architect](https://github.com/RinDig/icm-architect) · ICM paper: *Interpretable Context Methodology: Folder Structure as Agent Architecture* (Van Clief & McDermott).

See [NOTICE](NOTICE) for attribution details and [LICENSE](LICENSE) for the upstream MIT license.
