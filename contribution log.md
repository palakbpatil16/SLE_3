5. Code Level Overview:

Maze Representation: maze, ROWS, COLS

Position Finding: find_position(symbol) – finds the starting and goal positions.

Neighbor Finding: get_neighbors(row, col) – returns valid neighboring cells.

BFS Algorithm: bfs(start, goal) – uses a queue and visited set to search for the goal.

DFS Algorithm: dfs(start, goal) – uses a stack and visited set to search for the goal.

Node Counting: nodes_expanded – counts the number of nodes explored by each algorithm.

Profiling: profile_search.py runs BFS and DFS 10,000 times to observe their performance.
