# 🧭 A* Pathfinding Visualizer – Python & Pygame

An interactive **A\* pathfinding algorithm visualizer** built using **Python** and **Pygame**. This project provides a real-time, graphical demonstration of how the A* algorithm explores a grid, evaluates costs, and discovers the shortest path between two points while avoiding obstacles.

Designed as both a **learning tool** and a **portfolio project**, it highlights algorithmic thinking, data structures, and interactive visualization.

---

## 📌 Project Overview
The application allows users to:
- Place a **start node** and **end node** on a grid
- Draw **barriers (obstacles)** interactively
- Visually observe how the **A\*** algorithm explores nodes
- See the final shortest path reconstructed step by step

Each stage of the algorithm (open set, closed set, path) is color-coded for clarity.

---

## 🧠 Algorithm Implemented
**A\* Search Algorithm** with:
- Manhattan distance heuristic
- Priority queue–based open set
- Cost tracking using `g_score` and `f_score`
- Backtracking path reconstruction

This implementation guarantees the shortest path on a grid with uniform movement cost.

---

## 🎮 Controls & Interaction
| Action | Input |
|---|---|
| Place start node | Left-click (first click) |
| Place end node | Left-click (second click) |
| Draw barriers | Left-click (after start & end) |
| Remove node / barrier | Right-click |
| Run A* algorithm | Spacebar |
| Clear grid | C key |
| Quit | Close window |

---

## 🎨 Color Legend
| Color | Meaning |
|---|---|
| Orange | Start node |
| Turquoise | End node |
| Black | Barrier |
| Green | Open set |
| Red | Closed set |
| Purple | Final path |
| White | Empty node |

---

## 📁 File Structure
```text
astar_visualizer/
│
├── astar.py            # Main application and algorithm implementation
```

---

## 🧩 Code Architecture

### `Node` Class
Represents each cell in the grid and handles:
- Position and state
- Color-based visualization
- Neighbor detection (up, down, left, right)

### A* Algorithm (`algorithm` function)
- Uses a priority queue for efficient node selection
- Tracks path using `came_from` mapping
- Updates grid visualization in real time

### Rendering System
- Grid and node drawing via Pygame
- Frame-by-frame updates for algorithm animation

---

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- Pygame

Install dependency:
```bash
pip install pygame
```

---

## ▶️ Running the Visualizer
```bash
python astar.py
```

---

## 📈 Skills Demonstrated
- Graph search algorithms (A*)
- Heuristics and cost functions
- Priority queues and hash sets
- Interactive GUI development with Pygame
- Real-time algorithm visualization

---

## 🧪 Learning Outcomes
- Deep understanding of A* internals
- Visual intuition for open/closed sets
- Translating abstract algorithms into interactive systems
- Clean separation of logic and rendering

---

## 🏷️ Portfolio Note
This project demonstrates strong fundamentals in:
- **Algorithms & Data Structures**
- **Problem-solving and optimization**
- **Interactive visualization design**

---

## 🔮 Possible Enhancements
- Diagonal movement support
- Weighted nodes
- Multiple heuristic comparisons
- Performance metrics overlay

---

**Author:** Spondan Bandyopadhyay

---
