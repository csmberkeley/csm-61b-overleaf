# Balance a BST

Imagine being given a BST and asked to write a method to balance it. This sounds like a task so complex that B-Trees and LLRBs were invented for. In a normal BST, the only requirement is right children are larger and left children are smaller than the parent (as well as previous parents). Now we'll look at a simpler way to balance a BST that abuses space complexity.

1. How could you modify the tree with O(N) space to make this into a sorted array — which traversal?

2. What would be the time complexity of the above operation.


Solutions:
1. An In-Order Traversal should yield a sorted array.
2. An In-Order Traversal takes O(N) time. A common misconception is that sorting/balancing is O(NlogN) time but with a pre-maintained search-tree structure, it is O(N).
