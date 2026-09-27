# LeetCode 310 - Minimum Height Trees

## Problem Statement

Given a tree with `n` nodes and `n - 1` edges, find all possible roots that produce Minimum Height Trees.

Return the root labels.

## Example 1

### Input

```text id="8udlku"
n = 4
edges = [[1,0],[1,2],[1,3]]
```

### Output

```text id="h0g7t5"
[1]
```

## Example 2

### Input

```text id="0v4h7v"
n = 6
edges = [[3,0],[3,1],[3,2],[3,4],[5,4]]
```

### Output

```text id="8a2f2h"
[3,4]
```

## Approach

Use **Topological Trimming** by repeatedly removing the leaf nodes.

The center of a tree produces the minimum possible height. A tree can have one or two centers.

## Algorithm

1. Build an adjacency list for the tree.
2. Find all nodes with degree `1`.
3. Add these leaf nodes to a queue.
4. Remove the leaves layer by layer.
5. Update the degree of their neighbors.
6. Continue until at most two nodes remain.
7. Return the remaining nodes.

## Time Complexity

`O(n)`

## Space Complexity

`O(n)`

## Key Concepts

* Graph
* Tree
* BFS
* Topological Trimming
* Degree of Nodes
* Queue

## Language

Python

## LeetCode Details

* **Problem:** 310
* **Title:** Minimum Height Trees
* **Difficulty:** Medium

## Author

**T. Nandhini Reddy**

GitHub: `242t605119-dotcom`
