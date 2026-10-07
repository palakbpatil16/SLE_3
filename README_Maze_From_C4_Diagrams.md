# Grid-Based Maze Solving System using BFS and DFS

## Project Overview

The Grid-Based Maze Solving System is an Artificial Intelligence project that searches a grid-based maze using Breadth-First Search (BFS) and Depth-First Search (DFS). The system takes a maze as input, explores possible cells, checks for the goal, and provides the search result.

## System Architecture

The project architecture is represented using the diagrams below.

### 1. Context Diagram

The context diagram shows the main **Maze Solving System (Grid + BFS/DFS)** and its output, **Path / Result**. The system searches the maze and provides the result of the search.

### 2. Container Diagram

The container diagram shows the main parts of the system:

- **Maze/Grid Input Management:** Represents and manages the maze input.
- **Search Engine:** Performs the search using BFS and DFS.
- **Visited / Path Memory:** Keeps track of visited cells and path-related information during search.
- **Maze Solving System:** The overall system that connects these parts and produces the result.

### 3. Component Diagram

The component diagram focuses on the Search Engine and shows these components:

- **BFS / Queue:** Uses a queue to explore cells level by level.
- **DFS / Stack:** Uses a stack to explore a path deeply before exploring other paths.
- **Goal Test:** Checks whether the current cell is the goal.
- **Reconstruction:** Represents the path-reconstruction part of the design, if path details are maintained by the implementation.

## Algorithms Used

### Breadth-First Search (BFS)

BFS explores neighboring cells level by level and uses a queue to manage the cells waiting to be explored.

### Depth-First Search (DFS)

DFS explores one path deeply before exploring other available paths and uses a stack to manage the search.

Both methods can use a visited set to avoid exploring the same cell repeatedly.

## Main Code Elements

The Python implementation uses the following main elements:

- `maze` — stores the grid.
- `ROWS` and `COLS` — store the grid dimensions.
- `find_position(symbol)` — finds a symbol such as the start or goal.
- `get_neighbors(row, col)` — finds valid neighboring cells.
- `bfs(start, goal)` — performs Breadth-First Search.
- `dfs(start, goal)` — performs Depth-First Search.
- `nodes_expanded` — counts the nodes explored by the search.

## Performance Profiling

The `profile_search.py` file runs BFS and DFS repeatedly, 10,000 times each, to observe their repeated execution. This profiling script prints completion messages after each set of runs.

## Project Files

```text
Maze-SLE-2/
├── bfs_dfs.py
├── profile_search.py
└── README.md
```

- `bfs_dfs.py` contains the maze, helper functions, BFS, DFS, and the main program.
- `profile_search.py` imports the search functions and runs each algorithm 10,000 times.

## How to Run

Run the maze-solving program:

```bash
python bfs_dfs.py
```

Run the profiling program:

```bash
python profile_search.py
```

## Student Information

- **Name:** Palak Babaso Patil
- **PRN:** 25UAM093
- **Program:** SY B.Tech CSE (AI & ML)
- **Course:** 02AML204 – Introduction to Artificial Intelligence

## Conclusion

The diagrams describe the maze-solving system at three levels: context, containers, and components. The system uses BFS and DFS to search the grid, while the queue, stack, goal test, and visited/path memory represent the main parts involved in the search. The architecture helps explain how the maze input, search process, and result fit together.
