# Python Raycasting FPS

A Doom-style first-person game built with Python and Pygame as a learning project following a tutorial. It uses a two-dimensional map and raycasting to create a three-dimensional-looking world.

## Features

- Raycast wall rendering and textured environments.
- Keyboard movement, mouse look, and wall collision detection.
- Animated sprites and enemies.
- Weapon firing and reload animation.
- Enemy navigation using breadth-first search on a grid.
- Player health, gradual health recovery, and game-over restart.
- Sound effects.

## Run Locally

Use Python 3.10 or newer with a desktop display and audio support.

```bash
git clone https://github.com/OsmanMur/Doom-like-game-python.git
cd Doom-like-game-python
python -m venv .venv
```

Activate the environment:

- macOS/Linux: `source .venv/bin/activate`
- Windows: `.venv\Scripts\activate`

Then install Pygame and start the game from the repository root:

```bash
python -m pip install pygame
python main.py
```

Keep the bundled resources in place: the game loads its images and sounds using relative paths.

## Controls

| Input | Action |
| --- | --- |
| W / S | Move forward / backward |
| A / D | Strafe left / right |
| Mouse | Look left / right |
| Left mouse button | Fire |
| Escape | Quit |

## Code Guide

| File | Responsibility |
| --- | --- |
| `main.py` | Game initialization, event handling, update, and draw loop |
| `settings.py` | Display, player, mouse, and raycasting settings |
| `map.py` | Grid map |
| `player.py` | Movement, collisions, mouse input, and health |
| `raycasting.py` | Raycasting calculations |
| `object_renderer.py` | Scene rendering |
| `sprite_object.py` | Sprite animation |
| `object_handler.py` | Game objects and enemies |
| `npc.py` | Enemy behavior |
| `pathfinding.py` | Grid graph and breadth-first search |
| `weapon.py` | Weapon behavior |
| `sound.py` | Sound loading and playback |

## Learning Focus

This tutorial-based project helped me practice object-oriented Python, game loops, raycasting, collision detection, animation, and graph traversal. It is a learning recreation rather than an original game engine or official Doom release.

The repository also includes browser-build artifacts under `build/`; the instructions above describe the desktop Python entry point.
