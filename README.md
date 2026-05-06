# CADMUS

CADMUS is a graphics-focused project that combines **ShaderLab**, **C#**, **GLSL**, and **HLSL** to explore and implement real‑time rendering techniques.

> Language mix (by repository bytes): ShaderLab (67.4%), C# (23.4%), GLSL (7.1%), HLSL (2.1%).

## What’s in this repo
- **ShaderLab / HLSL**: Unity shader definitions and GPU programs.
- **C#**: Runtime and editor-side scripts that drive materials/shaders, rendering passes, and tooling.
- **GLSL**: Supporting shaders or reference implementations (e.g., for comparison, portability, or experimentation).

## Getting started

### Prerequisites
- **Unity** (recommended): This repository appears shader- and C#-heavy in a way that commonly maps to Unity projects. Use a Unity version compatible with the project settings in the repo (see `ProjectSettings/ProjectVersion.txt` if present).
- A GPU capable of running modern shaders (DX11+/Metal/Vulkan).

### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/Espartaneal/CADMUS.git
   cd CADMUS
   ```
2. Open the project in **Unity Hub** (Add project → select the repo folder).
3. Let Unity import assets and compile scripts.

## Running / Using CADMUS
Because repository layouts differ, here are common entry points:
- Look for a **sample scene** under `Assets/` (e.g., `Assets/Scenes/`), then open and press **Play**.
- Look for a **Demo** folder or prefabs showcasing shader effects.
- If the project uses custom render pipelines (URP/HDRP/custom SRP), check:
  - `Assets/Settings/`
  - `Assets/RenderPipeline/`
  - `ProjectSettings/GraphicsSettings.asset`

## Development notes
- **ShaderLab** files typically end in `.shader` and may include HLSL blocks.
- **HLSL** files often end in `.hlsl` / `.cginc` / `.shaderinclude`.
- **GLSL** files often end in `.glsl`, `.vert`, `.frag`.
- Keep shader variants and keywords under control—small changes can increase build time.

## Structure (typical)
If your repo follows common Unity conventions, you may see:
- `Assets/` — materials, shaders, scripts, scenes
- `Packages/` — package manifest and dependencies
- `ProjectSettings/` — Unity project settings

## Troubleshooting
- **Pink materials / shaders not compiling**: Check the Console for shader errors; verify the active render pipeline (Built‑in/URP/HDRP) matches the shaders.
- **Compilation errors in C#**: Ensure all required packages are installed (Window → Package Manager) and that scripting define symbols match expectations.
- **Platform differences**: Some shader code paths differ between DX11/12, Metal, Vulkan. Try switching target platform or graphics API.

## Contributing
Pull requests and issues are welcome.
- Create an issue describing the bug/feature.
- Prefer small, focused PRs.
- Include screenshots or captures for rendering changes.

## License
No license file has been detected by this README. If you intend this project to be open source, consider adding a `LICENSE` file (e.g., MIT, Apache-2.0, GPL-3.0).

## Acknowledgements
If you’re experimenting with or re-implementing known techniques (PBR, SDFs, post-processing, etc.), consider listing references/papers here.
