# Architecture and code sets

Civilian 66 is organized as Unreal Engine C++ modules with one-way dependencies. Shared contracts sit below gameplay domains; project-specific composition sits above them. User interface code presents domain state and submits requests rather than owning game rules.

| Code set | Responsibility |
|---|---|
| `C66Foundation` | Shared identifiers, tags, messages, and save contracts |
| `C66Control` | Player input, camera, and interaction intent |
| `C66Gameplay` | Reusable character, equipment, and action systems |
| `C66Economy` | Inventory, items, transactions, and crafting concepts |
| `C66Progression` | Progression and authorization concepts |
| `C66World` | World layout, mining data, and persistence concepts |
| `C66Ecology` | Reusable creature and encounter systems |
| `C66Game` | Civilian 66-specific game composition |
| `C66UI` | Presentation and player-facing views |

These descriptions are intentionally high level. Detailed designs, source implementations, maps, and campaign material remain in the private production repository.

## Current public scope

The project is built around an Unreal-native modular codebase and authored world content. This repository does not include a playable build or production source code. Module names indicate architectural areas, not a claim that all planned systems are complete.
