# StarCraft 2 Editor Skillset

A collection of GitHub Copilot agents and skills for StarCraft 2 map development in VS Code — covering Galaxy scripting, the SC2 Data Editor, AI, UI, units, effects, actors, and more.

## Installation

### Copilot CLI / Claude Code

```
/plugin install sc2-editor@<your-github-username>/Starcraft-2-editor-skillset
```

Then confirm everything loaded:

```
/skills
/agents
```

### VS Code (manual)

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
| `galaxy-spawner-wave` | Spawner, wave, and camp systems |
| `galaxy-ui-designer` | Dialogs, HUD, scoreboards, hero selection |
| `sc2-teacher` | Explains how things work; troubleshoots editor problems |
| `sc2data-designer` | Design full data chains (heroes, abilities, effects, actors) |
| `sc2data-expert` | General SC2 Data Editor (XML) expert |

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
| `sc2data-units-abilities` | Units, abilities, movers, turrets (XML) |
| `sc2data-effects-weapons` | Effects, weapons, upgrades, damage chain (XML) |
| `sc2data-behaviors-validators` | Behaviors, buffs, validators (XML) |
| `sc2data-actors-visuals` | Actors, animations, sounds, actor events (XML) |
