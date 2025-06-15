# A* Pathfinding Algorithm Visualizer (Grid-based using Pygame)

##  A* Algorithm - Concept

The **A\*** (A-Star) algorithm is a powerful pathfinding and graph traversal technique used in many applications like games, robotics, and maps. It is widely known for its performance and accuracy because it combines features of Dijkstra’s Algorithm and Greedy Best-First Search.

It uses the following cost function to determine the most efficient path:

```
f(n) = g(n) + h(n)
```

- `f(n)`: Total estimated cost of the cheapest solution through node `n`
- `g(n)`: Exact cost from the start node to node `n`
- `h(n)`: Heuristic — estimated cost from node `n` to the goal (we use Manhattan distance)

By evaluating both the cost to reach a node and the estimated cost to get to the goal, A* finds the most optimal path if one exists.

---

##  Features

- Interactive grid-based visualizer
- Set start and end nodes with right-click
- Place or remove obstacles with left-click
- Visualize the shortest path in real-time using A* Algorithm
- Clean and easy-to-understand user interface
- Efficient implementation using NumPy arrays

---



##  Technologies Used

- Python
- [Pygame](https://www.pygame.org/news)
- NumPy

---

##  How It Works

1. **Green Box** → Start Node (Right-click to place)
2. **Orange Box** → End Node (Right-click to place)
3. **Black Boxes** → Obstacles (Left-click to add)
4. **Blue Path** → Shortest path from start to end
5. **Left-click again** on obstacles to remove them
6. Press `Space` to start the algorithm
7. Press `C` to clear the grid and reset

---

## Installation

```bash
# Clone the repository
git clone https://github.com/YourUsername/Astar-Visualizer.git
cd Astar-Visualizer

# Create a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

>  Ensure you have Python 3.6 or above installed.

---

##  How to Run

```bash
python main.py
```

This will launch a window with the grid. You can now interact with it using your mouse and keyboard as described above.

---

##  Requirements

- Python 3.6+
- pygame
- numpy

You can install all dependencies via:

```bash
pip install pygame numpy
```

Or using:

```bash
pip install -r requirements.txt
```

---

##  Example Output

After placing start and end nodes and some obstacles, the shortest path is calculated and shown as:

```
[Start] → Blue path → [End]
```

The path dynamically avoids obstacles and always finds the least-cost solution if possible.

---

##  Controls Summary

| Action              | Mouse / Keyboard   |
|---------------------|--------------------|
| Set Start Node      | Right-click        |
| Set End Node        | Right-click        |
| Place Obstacle      | Left-click         |
| Remove Obstacle     | Left-click again   |
| Start A* Algorithm  | Spacebar           |
| Clear Grid          | C                  |

---

##  Algorithm Details

The **A\*** algorithm guarantees the shortest path if the heuristic is admissible (i.e., it never overestimates the cost to reach the goal). In this implementation, the **Manhattan Distance** is used as the heuristic because it's well-suited for grid-based movement.

---

##  License

This project is licensed under the [MIT License](LICENSE).

---


