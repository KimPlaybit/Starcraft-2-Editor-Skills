# StarCraft 2 Editor Skillset

A collection of GitHub Copilot agents and skills for StarCraft 2 map development in VS Code — covering Galaxy scripting, the SC2 Data Editor, AI, UI, units, effects, actors, and more.

## Installation

### Copilot CLI

```
/plugin install sc2-editor@KimPlaybit/Starcraft-2-editor-skillset
```

Then confirm everything loaded:

```
/skills
/agents
```

### Claude Code

This skillset can also be used with **Claude Code**.
Clone/download this repository and make the skillset available to Claude Code through the project's `your-project/.claude/` directory.
A simple project structure can look like:

```text
your-project/
├── .claude/
│   └── skills/
├── .agents/
├── .github/
└── ...
```

The `.agents/` and `.github/` folders are used by the GitHub Copilot setup described above. Claude Code uses `your-project/.claude/` for its own project-level skills.

```text
/skills
```
The same StarCraft 2 knowledge can then be used directly from Claude Code.

## VS Code (manual installation)

Copy the two folders into the **root of your own project**:

#### Copilot
```
.agents/       →  your-project/.agents/
.github/       →  your-project/.github/
```

#### Claude
```
.agents/             →  your-project/.agents/
.github/skills       →  your-project/.claude/skills
```

Open VS Code with GitHub Copilot Chat enabled — no further configuration required.

- Type `/agents` in Copilot Chat to list all available agents.
- Type `/skills` in Copilot Chat to list all available skills.

## What's Included

### Agents (`.github/agents/`)

| Agent | Purpose |
|---|---|
| `galaxy-expert` | General-purpose Galaxy scripting expert |
| `galaxy-ai-scripting` | AI behavior, waves, and tech tree in Galaxy |
| `galaxy-code-splitter` | Split monolithic scripts into modular files |
| `galaxy-combat-and-units` | Units, combat, behaviors, XP/leveling |
| `galaxy-naming-convention` | Audit and enforce Galaxy naming conventions |
| `galaxy-spawner-wave` | Spawner, wave, and camp systems |
| `galaxy-ui-designer` | Dialogs, HUD, scoreboards, hero selection |
| `sc2-localization-expert` | Localization files, missing translations, text audits |
| `sc2-teacher` | Explains how things work; troubleshoots editor problems |
| `sc2data-designer` | Design full data chains (heroes, abilities, effects, actors) |
| `sc2data-expert` | General SC2 Data Editor (XML) expert |
| `sc2data-wizard-expert` | Create and use Data Editor wizards (.BlizWiz) |

### Skills (`.agents/skills/`)

| Skill | Domain |
|---|---|
| `galaxy-language-fundamentals` | Core Galaxy syntax, types, and map init |
| `galaxy-code-organization` | File structure and modular layout |
| `galaxy-triggers-and-functions` | Triggers, events, async execution |
| `galaxy-units-and-groups` | Unit creation, behaviors, orders, death events |
| `galaxy-players-and-alliances` | Players, alliances, resources, cameras |
| `galaxy-ai-and-techtree` | AI waves, difficulty scaling, tech tree |
| `galaxy-game-systems` | Banks, spawners, revive, resource rewards |
| `galaxy-ui-and-dialogs` | Dialogs, frames, HUD messages, scoreboards |
| `galaxy-actor-and-visuals` | Actors, animations, tint, scale, opacity |
| `galaxy-sound-camera-environment` | Sound, music, camera, weather, lighting |
| `galaxy-points-regions-geometry` | Points, regions, pathfinding, coordinates |
| `galaxy-math-strings-conversion` | Math, type conversions, string formatting |
| `galaxy-debug-data-catalog` | Debug output, Data Table, Catalog access |
| `sc2-localization-and-text` | GameStrings, GameHotkeys, ObjectStrings, TriggerStrings |
| `sc2-units-reference` | Unit catalog reference — IDs, races, attributes, co-op commanders |
| `sc2data-units-abilities` | Units, abilities, movers, turrets (XML) |
| `sc2data-effects-weapons` | Effects, weapons, upgrades, damage chain (XML) |
| `sc2data-behaviors-validators` | Behaviors, buffs, validators (XML) |
| `sc2data-actors-visuals` | Actors, animations, sounds, actor events (XML) |
| `sc2data-wizards` | Data Editor wizards (.BlizWiz) for automating data creation (XML) |

---

## Also Recommended

If you're working with external packages or shared SC2 code, check out the **[SC2 Comet Package Manager](https://github.com/KimPlaybit/SC2-Comet-package-manager)** as well.

