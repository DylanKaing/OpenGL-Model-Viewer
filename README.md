# opengl-model-viewer

An interactive 3D shape viewer in C using OpenGL, with procedural geometry generation, mesh file loading, and a hand-built linear algebra library.

## What It Does

Renders 3D shapes in a 512x512 window with mouse-driven arcball rotation and scroll-to-zoom. Supports two modes:

- **Procedural generation** — builds a sphere, torus, and spring entirely from vertex math (rotation and translation matrices)
- **File loading** — reads mesh data from text files (bunny, falcon, Menger sponge, etc.) and auto-centers them in the viewport

Each triangle gets a random color, and back faces render as wireframe for visual depth.

## Controls

| Input | Action |
|-------|--------|
| `1` / `2` / `3` | Switch between sphere, torus, and spring |
| Left click + drag | Arcball rotation |
| Scroll wheel | Zoom in/out |
| `q` | Quit |

## Building and Running

```bash
make
./modelviewer
```

## Technologies

C, OpenGL, GLSL, GLEW, FreeGLUT
