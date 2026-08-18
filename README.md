# MOHLLEE

A single-file browser first-person shooter. Wave combat, ranged weapons, atmospheric
city-block environment.

## Run

Just open `index.html` in a modern browser. No build step.

```sh
python3 -m http.server 8080
# then visit http://localhost:8080/
```

## Controls

| Action | Desktop | Mobile |
|---|---|---|
| Move | W A S D | Left joystick |
| Look | Mouse | Right-side drag |
| Fire | Left click | Fire button |
| Jump | Space | ▲ button |
| Duck | Ctrl | ⇣ button |
| Sprint | Shift | ⇈ button |
| Reload | R | R button |
| Switch weapon | 1–5 | ⇆ button |

## Stack

- **Three.js** (via importmap) for the 3D scene
- Custom WebGL renderer
- Custom 2D canvas overlay for the HUD chrome (weapon viewmodel, tracers)
- No build, no npm, no framework. One HTML file.

## Files

- `index.html` — the game (single file)
- `Dockerfile` — nginx static-serve container for the host
