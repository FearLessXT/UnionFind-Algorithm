# The First Algorithm of Union Find.

- Dynamic connectivity
- Quick Find
- Quick Union
- Improvements
- Applications
  
  # Union Find Algorithm in Java

  This project implements the Union Find algorithm in Java.

  ## What is Union Find?

  Union Find is a Disjoint-Set data structure. It represents a collection of disjoint (non-overlapping) sets.

  The two main operations performed on these sets are:

  - `Union` - Merge two sets into one. 
  - `Find` - Determine which set a particular element belongs to.

  Union Find can be used to solve connectivity problems, detect cycles in graphs and perform hierarchical clustering.

  ## Implementation

  The implementation uses two classes:

  `Node` - Represents a node in the Union Find sets. It contains:

  - `data` - The data stored in the node
  - `parent` - Points to the parent node in the set

  `UnionFind` - Contains the main Union Find logic:

  - `union(int p, int q)` - Unites the sets containing p and q
  - `find(int p)` - Finds the representative of the set that p belongs to
  - `connected(int p, int q)` - Checks if p and q are in the same set

  The `find()` operation uses path compression to optimize the time complexity.

  Time complexity:

  - `find()`: O(α(n)) amortized due to path compression  
  - `union()`: O(1) 
  - `connected()`: O(1)

  Space complexity: O(n)

  ## How to run

  - Compile: `javac UnionFind.java`
  - Run: `java UnionFind` 

  This will run some sample test cases and demonstrate the Union Find operations.
