# Lunar Habitat 3D Models

Interactive glTF 2.0 models from the NASA HUNCH **Lunar Smart Adaptive Habitat** project, shown in the browser with `<model-viewer>`. Pick any model from the gallery, orbit and zoom it, download the `.glb`, or view it in AR on a phone.

**Live site:** https://jaigod.github.io/LunarHabitat-3D/
**Main project:** https://jaigod.github.io/LunarSmartAdaptiveHabitat/

Link straight to a model with its id, e.g. `https://jaigod.github.io/LunarHabitat-3D/#wellness-greenhouse`.

## What's in the gallery (82 models, 54 MB)

| Category | Models | Folder |
|---|---|---|
| Lunar Smart Adaptive Habitat | 3 | `models/` |
| Habitat designs (RICH_BAKED set + HUNCH Final Habitat) | 12 | `models/habitats/` |
| Base layouts (Project 1/2 and Project 3) | 3 | `models/bases/` |
| Wellness solutions | 23 | `models/wellness/` |
| Health monitoring | 6 | `models/health/` |
| LUNA VR modules | 14 | `models/luna/` |
| LUNA-X hero assets | 4 | `models/luna_x/` |
| 3D-print kits | 4 | `models/kits/` |
| Engineering modules | 3 | `models/engineering/` |
| NASA reference (NASA 3D Resources) | 10 | `models/nasa/` |

The list, titles, descriptions and camera settings live in [`models/catalog.json`](models/catalog.json); the page builds itself from that file. Thumbnails are in `thumbs/`.

## How the models were made

- Blender files and FBX scenes were exported to GLB with Blender 5.2; STL print parts were imported and colored by building type.
- Existing GLBs were optimized with gltf-transform.
- Everything uses Draco mesh compression. Very large scenes were decimated and their textures reduced for the web (HUNCH Final Habitat went from 7.4 million to about 0.8 million triangles).
- Every file passes the Khronos glTF Validator with 0 errors and was checked loading in the page.

You can open any `.glb` in VS Code with the glTF Tools extension to inspect or preview it.
