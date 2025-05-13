# 🐍 3D Pixel Python

Welcome to **3D Pixel Python**, a 3D pixel-style snake game developed in **Python** using **PyOpenGL** and **GLUT**. This project blends classic snake mechanics with modern 3D rendering and game logic for an engaging, dynamic experience.

---

## 🎮 Features

- ✅ Fully 3D-rendered Snake and Grid using OpenGL
- 🍎 Classic food and 💠 special power-ups (speed & double points)
- 💣 Bombs and 🧱 obstacles for challenging gameplay
- 🎚️ Multiple difficulty levels: Easy, Medium, Hard
- 🎥 Controllable camera (zoom, height, rotation)
- 🌈 Dynamic sky color transitions
- 📊 Score tracking and end-game feedback
- 🕹️ Responsive input: arrow keys, WASD, mouse clicks
- 🖥️ Clean UI with 2D overlays

---

## 🧰 Requirements

- Python 3.7+
- PyOpenGL

---

## 🕹️ Controls

### Snake Movement

| Action     | Key     |
| ---------- | ------- |
| Move Up    | ↑ Arrow |
| Move Down  | ↓ Arrow |
| Move Left  | ← Arrow |
| Move Right | → Arrow |

### Camera Controls

| Action                  | Key |
| ----------------------- | --- |
| Zoom In                 | `x` |
| Zoom Out                | `y` |
| Rotate Clockwise        | `d` |
| Rotate Counterclockwise | `a` |
| Raise Camera            | `w` |
| Lower Camera            | `s` |

### Game State

| Action         | Key/Button     |
| -------------- | -------------- |
| Pause / Resume | `p` or `Space` |
| Restart        | `r`            |
| Exit           | `Esc`          |
| UI Buttons     | Mouse click    |

---

## 🎯 Gameplay Mechanics

* Eating **food** increases your score and grows the snake.
* After 5 regular foods, a **special star** appears:
  * Collecting it speeds up the snake and activates **double points** for 10 seconds.
* **Bombs** spawn every few seconds depending on difficulty.
* **Obstacles** are generated in clusters and change over time.
* The **sky color** dynamically changes after certain score milestones.
* The snake wraps around edges of the grid.

---

## 🛠️ Code Architecture

| Component                                | Description                           |
| ---------------------------------------- | ------------------------------------- |
| `draw_grid`                              | Renders the 3D chessboard-style grid. |
| `draw_snake`                             | Renders the snake (head, body, tail). |
| `draw_food`, `draw_special_food`         | Renders normal and special foods.     |
| `draw_bombs`, `generate_bombs`           | Handles bomb visuals and logic.       |
| `draw_obstacles`                         | Draws fixed obstacle blocks.          |
| `setup_camera`, `display`                | Manages 3D rendering and view.        |
| `keyboardListener`, `specialKeyListener` | Handles keyboard input.               |
| `mouseListener`                          | Handles UI button clicks.             |
| `idle`                                   | Manages game updates and redraws.     |

---

## 📸 Screenshots

*Coming soon — upload gameplay images or short GIFs here.*

---

## 🧩 Known Limitations

* Snake direction is dependent on camera angle — ensure it's aligned to 0°, 90°, 180°, or 270° for accurate movement.
* Performance may vary depending on GPU and OpenGL support.

---

## 🙌 Acknowledgements

Inspired by the classic Nokia Snake game and extended into 3D using PyOpenGL.

---

## 👥 Contributors

- **Rauf & Team**

---
