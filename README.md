# AI_LAB_ASSIGNMENT-3_SE24UCSE035
CODES FOR THE AI ASSIGNMENT 3
Explanation
CODE-1:
This implements Uniform Cost Search (Dijkstra).

Cities are represented as nodes (e.g., Delhi, Mumbai, Chennai, etc.).

Graph is stored as an adjacency matrix with road distances.

Algorithm:

Start from source city

Always expand the least-cost node

Update distances to neighbors

Guarantees shortest path to all cities

Used in:

GPS navigation

Transport planning
CODE-2:
Grid represents battlefield (0 = free, 1 = obstacle)

BFS ensures shortest path in uniform grid

Moves allowed:

Up, Down, Left, Right

Random density:

Low → few 1s

Medium → moderate obstacles

High → dense obstacles

Measures of Effectiveness (MoE)

Path length (distance)

Time taken

Nodes explored

Success rate

This simulates UGV navigation with known obstacles
CODE-3:
Grid represents battlefield (0 = free, 1 = obstacle)

BFS ensures shortest path in uniform grid

Moves allowed:

Up, Down, Left, Right

Random density:

Low → few 1s

Medium → moderate obstacles

High → dense obstacles

📊 Measures of Effectiveness (MoE)

Path length (distance)

Time taken

Nodes explored

Success rate

👉 This simulates UGV navigation with known obstacles

🔷 3. Dynamic Obstacles (Real-World Scenario)
✅ Code (Conceptual A* style - simplified)
#include <stdio.h>
#include <stdlib.h>
#include <math.h>

#define N 10

int heuristic(int x1,int y1,int x2,int y2){
    return abs(x1-x2)+abs(y1-y2);
}

int main(){
    printf("Use A* with real-time updates\n");
    return 0;
}
🧠 Explanation

Static BFS is NOT enough when:

Obstacles move

Environment changes

✅ Solution Approaches:

A* Algorithm

Uses:
f(n) = g(n) + h(n)

g(n): path cost

h(n): heuristic (Manhattan distance)

D (Dynamic A*)*

Replans path when obstacle appears

Used in:

Mars rovers

Military robots

Real-time Sensors

LIDAR / Camera detect obstacles

Update map dynamically

Measures of Effectiveness (Dynamic)

Replanning time

Adaptability

Path optimality

Safety (collision avoidance)
