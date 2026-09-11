# LevelSync

Paper/Spigot plugin that synchronizes combat skill levels between **AuraSkills** and **EliteMobs**.

## Features

- **Skill Sync** – Bidirectionally keeps related AuraSkills / EliteMobs combat levels in sync
  - Defense (AuraSkills) ↔ Armor (EliteMobs)
  - Fighting (AuraSkills) ↔ Swords / Axes / Maces / Spears / Hoes (EliteMobs)
  - Archery (AuraSkills) ↔ Bows / Crossbows / Tridents (EliteMobs)
- Force-sync command and status GUI

## Requirements

| Plugin      | Role            |
|-------------|-----------------|
| Paper 1.21+ | Server          |
| AuraSkills  | Hard dependency |
| EliteMobs   | Hard dependency |

## Commands

| Command               | Permission         | Description                    |
|-----------------------|--------------------|--------------------------------|
| `/levelsync [player]` | `levelsync.admin`  | Force sync combat levels       |
| `/levelsyncgui`       | `levelsync.gui`    | Open Level Sync status GUI     |

## Permissions

- `levelsync.admin` – force sync (default: op)
- `levelsync.gui` – open GUI (default: true)

## Building

**Gradle**
```bash
gradle build
# or
./gradlew build
