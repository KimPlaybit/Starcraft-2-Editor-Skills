# StarCraft 2 Editor Skillset

A collection of GitHub Copilot and Claude Code agents and skills for StarCraft 2 map development in VS Code — covering Galaxy scripting, the SC2 Data Editor, AI, UI, units, effects, actors, and more.

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

The repository is also a Claude Code plugin marketplace. Add it and install the plugin:

```
/plugin marketplace add KimPlaybit/Starcraft-2-editor-skillset
/plugin install sc2-editor@sc2-editor-skillset
```

Then confirm everything loaded:

```
/skills
/agents
```

Claude Code reads `.claude-plugin/plugin.json`, which points at the same `.agents/skills/` and `.github/agents/` folders used by Copilot. No files are duplicated, so Copilot and Claude always share the same content.

## VS Code (manual installation)

Copy the two folders into the **root of your own project**:

```
.agents/       →  your-project/.agents/
.github/       →  your-project/.github/
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

### Adding new agents or skills

- **Skills:** drop a new folder with a `SKILL.md` into `.agents/skills/`. Both Copilot and Claude Code pick it up automatically.
- **Agents:** add the `*.agent.md` file to `.github/agents/` **and** list its path under `agents` in `.claude-plugin/plugin.json`, because Claude Code only accepts explicit agent file paths. Use a kebab-case `name:` in the frontmatter, for example `name: galaxy-expert`. Claude Code skips agents whose names contain spaces.

---

## Also Recommended

If you're working with external packages or shared SC2 code, check out the **[SC2 Comet Package Manager](https://github.com/KimPlaybit/SC2-Comet-package-manager)** as well.

