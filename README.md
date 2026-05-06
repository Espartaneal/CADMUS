# CADMUS

**CADMUS** is a **3D open‑world** action/survival game project where you explore a living world and fight back against an evil organization and its relentless **zombie hordes**.

The game is inspired by large-scale open-world adventures (in the “Genshin-like” sense of exploration and world systems), with a focus on atmosphere and simulation: **dynamic weather**, a **day/night cycle**, and diverse biomes.

## Core features (planned / in progress)
- **Open world exploration**: forests, lakes, villages, and interconnected areas.
- **Dynamic world systems**:
  - **Weather** (e.g., rain/overcast/clear)
  - **Day & night cycle** with different ambience and threats
- **Enemy encounters**: roaming enemies and **zombie hordes**.
- **Traversal & transport**: vehicles/transports to move across the world.
- **Combat**: firearms / guns.

## Tech snapshot
This repository is primarily a **Unity**-style mix of gameplay code and shader work:

> Language mix (by repository bytes): ShaderLab (67.4%), C# (23.4%), GLSL (7.1%), HLSL (2.1%).

- **C#**: gameplay systems, world logic, tools
- **ShaderLab / HLSL**: Unity shaders and rendering work
- **GLSL**: supporting shaders / experiments / references

## Getting started

### Prerequisites
- **Unity** (recommended). If this is a Unity project, the exact editor version is typically recorded in:
  - `ProjectSettings/ProjectVersion.txt`
- A GPU capable of modern real-time rendering (DX11+/Metal/Vulkan).

### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/Espartaneal/CADMUS.git
   cd CADMUS
   ```
2. Open the project in **Unity Hub** (Add project → select the repo folder).
3. Allow Unity to import assets and compile scripts.

### Run the game (in Editor)
- Open the project’s main scene (commonly under `Assets/Scenes/`) and press **Play**.

> If you tell me the exact “main” scene path, I can update this README to point to it directly.

## Project structure (typical)
If the repo follows standard Unity conventions:
- `Assets/` — materials, shaders, scripts, scenes
- `Packages/` — package manifest and dependencies
- `ProjectSettings/` — Unity project settings

## Roadmap ideas
- More biomes and points of interest (villages/ruins/roads)
- Horde/wave logic + POI defense events
- Wildlife / ambient AI
- Loot + crafting/upgrades
- Save/load

## Contributing
Issues and pull requests are welcome.
- Keep PRs small and focused.
- Include screenshots/video captures for rendering or world-visual changes.

## License
No license file is referenced here yet. If you plan to open source CADMUS, add a `LICENSE` file (e.g., MIT/Apache-2.0/GPL-3.0).
