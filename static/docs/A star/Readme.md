# Introduction

It is a searching algorithm that is used to find the shortest path between an initial and a final point.

A\* was initially designed as a graph traversal problem, to help build a robot that can find its own course. It still remains a widely popular algorithm for graph traversal.

It is an extension of Dijkstra’s shortest path algorithm (Dijkstra’s Algorithm). The extension here is that, instead of using a priority queue to store all the elements, we use heaps (binary trees) to store them.

The A\* Search Algorithm also uses a heuristic function that provides additional information regarding how far away from the goal node we are. This function is used in conjunction with the f-heap (Fibonacci heap) data structure in order to make searching more efficient.

It searches for shorter paths first, thus making it an optimal and complete algorithm.

- An optimal algorithm will find the least cost outcome for a problem.
- A complete algorithm finds all the possible outcomes of a problem.

# Working

Initially, the Algorithm calculates the cost to all its immediate neighboring nodes,n, and chooses the one incurring the least cost. This process repeats until no new nodes can be chosen and all paths have been traversed. Then, you should consider the best path among them. If f(n) represents the final cost, then it can be denoted as :

f(n) = g(n) + h(n), where :

g(n) = cost of traversing from one node to another. This will vary from node to node

h(n) = heuristic approximation of the node's value. This is not a real value but an approximation cost

Calculating g is not a big deal but to calculate h we can:

1. Calculate the exact value of h (which is certainly time consuming).
1. Approximate the value of h using some heuristics (less time consuming).
   - Manhattan Distance
   - Diagonal Distance
   - Euclidean Distance

We can also think of Dijkstra as a special case of A\* Search Algorithm, where h = 0 for all nodes.

# Complexity Analysis

TIME COMPLEXITY: O(E), where E is the number of edges in the graph
SPACE COMPLEXITY: O(V), where V is the total number of vertices.

# Limitations

A major drawback of the algorithm is its space and time complexity. It takes a large amount of space to store all possible paths and a lot of time to find them.

Although being the best path finding algorithm around, A\* Search Algorithm doesn’t produce the shortest path always, as it relies heavily on heuristics / approximations to calculate – h

A heuristic algorithm sacrifices optimality, with precision and accuracy for speed, to solve problems faster and more efficiently.
