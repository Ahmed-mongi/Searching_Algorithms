# Path-Finding Agent in a Binary Tree


## Project Overview
This project implements multiple path-finding algorithms to navigate a binary tree and locate a designated goal node. The binary tree serves as the search space, where each node represents a state, and movements occur between parent and child nodes.

## Problem Modeling
### State Space Representation
- The problem is modeled as a binary tree, with each node representing a state.
- Nodes have children representing possible moves.
- The tree is generated up to a predefined maximum depth to ensure manageable search space.

### Initial and Goal States
- **Initial State**: The root node at the top center of the tree.
- **Goal State**: A randomly selected leaf node containing an apple.

### Actions
- The agent moves from a parent node to one of its child nodes.
- Each move corresponds to an action taken to traverse the tree.

## Algorithms Implemented
- **Breadth-First Search (BFS)**: Explores the tree level by level to ensure the shortest path is found.
- **Depth-First Search (DFS)**: Explores as deep as possible along each branch before backtracking.
- **Uniform Cost Search (UCS)**: Finds the least costly path when step costs vary.
- **Iterative Deepening Search (IDS)**: Merges DFS space efficiency with BFS optimality.
- **Hill Climbing**: Uses a heuristic to move towards the best estimated next state.
- **Simulated Annealing**: Employs randomness to escape local optima and find better paths.
- **A* Search**: Uses cost and heuristic functions to efficiently find the optimal path.
- **Genetic Algorithm**: Evolves solutions using crossover and mutation to locate the goal.

## Performance Summary
| Algorithm        | Strengths | Weaknesses |
|-----------------|------------|------------|
| **BFS** | Finds the shortest path | Slow for deep trees |
| **DFS** | May find a solution quickly | Not guaranteed to find the shortest path |
| **UCS** | Guarantees optimality for varying costs | Similar to BFS when costs are uniform |
| **IDS** | Balances space efficiency and optimality | Can be slow due to repeated searches |
| **Hill Climbing** | Fast, heuristic-driven | Can get stuck in local optima |
| **Simulated Annealing** | Escapes local optima | Requires careful parameter tuning |
| **A* Search** | Finds optimal path efficiently | Dependent on heuristic quality |
| **Genetic Algorithm** | Can discover good solutions through evolution | Requires careful tuning of parameters |

## Analysis and Reflections
- **BFS and UCS** reliably find the shortest path but are slower due to exhaustive searching.
- **DFS** may provide quick solutions but isn't guaranteed to be optimal.
- **IDS** balances time and space efficiency but is slower due to repetition.
- **Hill Climbing and Simulated Annealing** require careful tuning and heuristic selection to be effective.
- **A* Search** is the most efficient when a good heuristic is available.
- **Genetic Algorithm** can perform well but depends on population size and mutation rate.

## Installation and Usage
### Requirements
- Python 3.x
- Required libraries (install via `pip install -r requirements.txt` if applicable)

### Running the Project
1. Clone this repository:
   ```sh
   git clone https://github.com/yourusername/path-finding-agent.git
   cd path-finding-agent
   ```
2. Run the script:
   ```sh
   python main.py
   ```
3. Choose an algorithm to execute and observe the path-finding process.


## License
This project is open-source and available under the MIT License.

