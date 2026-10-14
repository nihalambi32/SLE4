# SLE4
SLE-4: Architecture Decision Record (ADR)
Student Details
Course: 02AML204 – Introduction to Artificial Intelligence
PRN: 25UET106
Name: Nihal Ambi
Division: B
Decision Status: Accepted
1. Title
Use Breadth-First Search (BFS) as the Main Solver for Maze Path-Finding
2. Context
The project compares Breadth-First Search (BFS) and Depth-Limited Depth-First Search (DFS) for solving grid mazes. The maze has a start point at the top-left and a goal at the bottom-right. The algorithms were tested on maze sizes of 20×20, 40×40, and 70×70. The project records path length, execution time, and expanded nodes.
3. Decision
Use BFS as the main algorithm when the shortest path is required. Keep DFS for comparison.
4. Alternatives Considered
BFS: Explores nodes level by level and finds a shortest path in an unweighted maze.
Depth-Limited DFS: Explores a path deeply up to a limit, but does not guarantee the shortest path.
5. Rationale
The SLE-2 README reports the following results:
Maze Size
BFS Path Length
DFS Path Length
BFS Nodes Expanded
DFS Nodes Expanded
20×20
38
72
295
155
40×40
78
166
1,212
674
70×70
138
390
3,739
2,421
BFS found shorter paths in all three reported cases. DFS expanded fewer nodes in these cases. Results can vary because the mazes are randomly generated.
6. Consequences
Advantages
BFS finds the shortest path in an unweighted maze.
The project can compare path length, execution time, and expanded nodes.
Disadvantage
BFS expanded more nodes than DFS in the reported test cases.
7. Summary of Earlier SLE Projects
SLE-1: Student AI Assistant
A Python-based, rule-based assistant that responds to student questions about topics such as Python, DSA, exams, college, and study tips. GitHub Copilot was used for selected code sections, and the student reviewed and tested the suggestions.
Repository: https://github.com/nihalambi32/IAI
SLE-2: BFS vs DFS
Compares BFS and Depth-Limited DFS on mazes of sizes 20×20, 40×40, and 70×70. It records execution time and expanded nodes and compares the path lengths.
Repository: https://github.com/nihalambi32/SLE-2
SLE-3: C4 Architecture
Documents the maze project's architecture. The listed components are Maze Generator, Search Engine, Path Reconstructor, Output & Metrics, and Experiment & Profiling.
Repository: https://github.com/nihalambi32/SLE-3
8. AI Contribution Note
GitHub Copilot was used in SLE-1 for selected code sections. The contribution log records suggestions for parts of the student_agent() structure and response handling. The student reviewed, tested, and modified the code.
9. References
SLE-1: https://github.com/nihalambi32/IAI
SLE-2: https://github.com/nihalambi32/SLE-2
SLE-3: https://github.com/nihalambi32/SLE-3
