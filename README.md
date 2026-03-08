# Labyrinth Drift

A simple **world exploration** game built with the **Unity 3D** engine. Control a 3D avatar and explore a **procedurally generated maze** with walls, rooms, doors, trees, stairs, and more. The maze is never the same twice and expands as you explore—reaching the edge triggers generation of new content for an effectively endless world.

![Image of Labyrinth Drift](http://cdn.rawgit.com/erikbuck/MazeVenture/master/MazeVenture.png)

---

## Features

- **Procedural maze generation** — Each playthrough produces a unique layout
- **Multi-level mazes** — Stairs connect different elevations with landings and railings
- **Rooms and doors** — Connected spaces with configurable door probability
- **Decorations** — Trees, wall variants, columns, and banisters
- **Smooth player movement** — Grid-based movement with walk/run and directional facing
- **Third-person view** — Camera follows the player through the maze

---

## Technology

- **Engine:** Unity 3D
- **Language:** C#
- **Content:** Custom 3D models and scripts plus free assets from the Unity Asset Store (e.g. Yurowm character/animations, SpeedTree-style trees)

---

## Getting Started

### Requirements

- **Unity** (version compatible with the project; typically Unity 5.x or later for this codebase)

### Running the Project

1. Clone or download this repository.
2. Open the project folder in **Unity Hub** or Unity (Open Project → select the project root).
3. Open the main scene: `Assets/Scene.unity`.
4. Press **Play** in the Unity Editor.

### Controls

| Key | Action |
|-----|--------|
| **W** / **↑** | Move forward |
| **S** / **↓** | Move backward |
| **A** / **←** | Move / turn left |
| **D** / **→** | Move / turn right |
| **Q** | Turn left (in place) |
| **E** | Turn right (in place) |
| **Space** | Restart game (new maze) |

The player automatically walks or runs depending on distance to the next cell. Movement is grid-based: one keypress advances one cell in the chosen direction.

---

## Project Structure

```
LabyrinthDrift/
├── Assets/
│   ├── Scene.unity              # Main game scene
│   ├── Scripts/                # Core C# game logic
│   │   ├── GameManager.cs      # Maze + player setup, restart
│   │   ├── Player.cs          # Movement, routing, input
│   │   ├── Maze.cs            # Procedural generation
│   │   ├── MazeCell.cs        # Cell data and edges
│   │   ├── MazePassage.cs     # Open passages
│   │   ├── MazeDoor.cs        # Doors between rooms
│   │   ├── MazeStairs.cs      # Stairs and landings
│   │   ├── MazeWall.cs        # Walls and railings
│   │   ├── MazeDirection.cs   # Cardinal directions
│   │   ├── IntVector2.cs     # 2D integer coordinates
│   │   └── ...
│   ├── Prefabs/               # Maze and player prefabs
│   ├── Materials/             # Wall, floor, door materials
│   ├── Yurowm/                # Character & animations (Asset Store)
│   └── Free_SpeedTrees/       # Tree assets
├── LICENSE.md
└── README.md
```

---
