# Uninformed Search / Blind Search

![Image](../../images/blind-search-01.png)

![Image](../../images/uniform-search-01.png)

<br/>

- Try to go in every path and find the best path to get the final goal state
- These are brute force search algorythms
- It doesnt use information about the problem to guide search
- Not very efficient
- Take long time to achieve

<br/>

## Key evaluation criteria:

- `Completeness`: Does it always find a solution if one exists?

- `Time Complexity`: How long does it take to find a solution?

- `Space Complexity`: How much memory is required?

- `Optimality`: Does it find the lowest-cost/shortest path?

<br/>

## Algorythms

- [Breadth-First-Search | BFS](./bfs.md)
- [Depth-First-Search | DFS](./dfs.md)
- [Uniform-Cost-Search | UCS](./ucs.md)
- [Depth-Limited-Search | DLS](./dls.md)
- Iterative Deeping Depth First Search
- Bidirectional Search

---

## Uninformed Search Algorithms: Quick Comparison Summary

| Algorithm | Complete? | Optimal? | Time Complexity | Space Complexity | Main Data Structure |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Breadth-First Search (BFS)** | Yes | Yes* | $O(b^d)$ | $O(b^d)$ | FIFO Queue |
| **Depth-First Search (DFS)** | No | No | $O(b^m)$ | $O(bm)$ | LIFO Stack |
| **Uniform Cost Search (UCS)** | Yes | Yes | $O(b^{1 + C^*/\epsilon})$ | $O(b^{1 + C^*/\epsilon})$ | Priority Queue ($g(n)$) |
| **Depth-Limited Search (DLS)** | No ($l < d$) | No | $O(b^l)$ | $O(bl)$ | Stack with Depth Limit |

*\*Optimal only if all step costs are equal.*
