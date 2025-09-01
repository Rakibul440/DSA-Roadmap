# Complete Data Structures and Algorithms Reference

## Linear Data Structures

### 1. Arrays
**Features:**
- Fixed size collection of elements
- Elements stored in contiguous memory locations
- Random access using index
- Cache-friendly due to locality of reference

**Types:**
- Static Arrays (fixed size)
- Dynamic Arrays (resizable)
- Multi-dimensional Arrays
- Jagged Arrays

**Operations:**
- Access: O(1)
- Search: O(n) linear, O(log n) if sorted
- Insertion: O(n) worst case, O(1) at end
- Deletion: O(n) worst case, O(1) at end

### 2. Linked Lists
**Features:**
- Dynamic size
- Elements stored in nodes with pointers
- Sequential access only
- Efficient insertion/deletion at any position

**Types:**
- Singly Linked List
- Doubly Linked List
- Circular Linked List
- Doubly Circular Linked List

**Operations:**
- Access: O(n)
- Search: O(n)
- Insertion: O(1) if position known, O(n) otherwise
- Deletion: O(1) if position known, O(n) otherwise

### 3. Stacks
**Features:**
- Last In First Out (LIFO) principle
- Operations performed at one end (top)
- Used for function calls, expression evaluation, undo operations

**Operations:**
- Push: O(1)
- Pop: O(1)
- Peek/Top: O(1)
- isEmpty: O(1)

**Applications:**
- Function call management
- Expression evaluation and syntax parsing
- Backtracking algorithms
- Browser history
- Undo functionality

### 4. Queues
**Features:**
- First In First Out (FIFO) principle
- Operations at both ends (front and rear)
- Used for scheduling, buffering

**Types:**
- Simple Queue
- Circular Queue
- Priority Queue
- Double-ended Queue (Deque)

**Operations:**
- Enqueue: O(1)
- Dequeue: O(1)
- Front: O(1)
- Rear: O(1)
- isEmpty: O(1)

## Non-Linear Data Structures

### 5. Trees
**Features:**
- Hierarchical structure
- One root node
- Nodes connected by edges
- No cycles

**Types:**

#### Binary Trees
- Each node has at most 2 children
- Left and right child
- Subtypes: Complete, Full, Perfect, Balanced

#### Binary Search Trees (BST)
- Left subtree values < root < right subtree values
- Efficient searching, insertion, deletion

#### AVL Trees
- Self-balancing binary search tree
- Height difference between left and right subtrees ≤ 1
- Rotations to maintain balance

#### Red-Black Trees
- Self-balancing binary search tree
- Each node colored red or black
- Satisfies red-black properties

#### B-Trees
- Self-balancing search tree
- Multiple keys per node
- Used in databases and file systems

#### B+ Trees
- Variant of B-tree
- All values stored in leaf nodes
- Internal nodes store only keys

#### Trie (Prefix Tree)
- Tree for storing strings
- Each path represents a word
- Efficient for prefix searches

#### Segment Trees
- Binary tree for range queries
- Each node stores information about a range
- Supports range sum, min, max queries

#### Fenwick Tree (Binary Indexed Tree)
- Efficient for prefix sums
- Update and query in O(log n)

**Tree Operations:**
- Search: O(log n) balanced, O(n) worst case
- Insertion: O(log n) balanced, O(n) worst case
- Deletion: O(log n) balanced, O(n) worst case

**Tree Traversals:**
- Preorder (Root, Left, Right)
- Inorder (Left, Root, Right)
- Postorder (Left, Right, Root)
- Level Order (Breadth First)

### 6. Heaps
**Features:**
- Complete binary tree
- Heap property maintained
- Efficient for priority operations

**Types:**
- Max Heap (parent ≥ children)
- Min Heap (parent ≤ children)
- Binary Heap
- Binomial Heap
- Fibonacci Heap
- d-ary Heap

**Operations:**
- Insert: O(log n)
- Extract Min/Max: O(log n)
- Peek: O(1)
- Decrease Key: O(log n)
- Build Heap: O(n)

### 7. Graphs
**Features:**
- Collection of vertices and edges
- Can represent complex relationships
- Directed or undirected

**Types:**
- Directed Graph (Digraph)
- Undirected Graph
- Weighted Graph
- Unweighted Graph
- Cyclic Graph
- Acyclic Graph
- Connected Graph
- Disconnected Graph
- Complete Graph
- Bipartite Graph

**Representations:**
- Adjacency Matrix: O(V²) space
- Adjacency List: O(V + E) space
- Edge List: O(E) space

**Operations:**
- Add Vertex: O(1)
- Add Edge: O(1)
- Remove Vertex: O(V + E)
- Remove Edge: O(V) or O(1) depending on representation

## Hash-Based Data Structures

### 8. Hash Tables
**Features:**
- Key-value pairs
- Fast access using hash function
- Average O(1) operations

**Collision Resolution:**
- Chaining (using linked lists)
- Open Addressing (linear probing, quadratic probing, double hashing)
- Robin Hood Hashing
- Cuckoo Hashing

**Operations:**
- Insert: O(1) average, O(n) worst case
- Delete: O(1) average, O(n) worst case
- Search: O(1) average, O(n) worst case

### 9. Bloom Filters
**Features:**
- Probabilistic data structure
- Tests membership in a set
- False positives possible, no false negatives
- Space efficient

## Advanced Data Structures

### 10. Disjoint Set Union (Union-Find)
**Features:**
- Tracks disjoint sets
- Supports union and find operations
- Used in Kruskal's algorithm, connected components

**Optimizations:**
- Path Compression
- Union by Rank/Size

**Operations:**
- Find: O(α(n)) with optimizations
- Union: O(α(n)) with optimizations

### 11. Suffix Trees and Arrays
**Suffix Tree Features:**
- Compressed trie of all suffixes
- Linear space and construction time
- Efficient substring operations

**Suffix Array Features:**
- Sorted array of suffix positions
- Space efficient alternative to suffix trees

### 12. Skip Lists
**Features:**
- Probabilistic data structure
- Multiple levels of linked lists
- Alternative to balanced trees
- Average O(log n) operations

## Sorting Algorithms

### Comparison-Based Sorts

#### 1. Bubble Sort
- Time: O(n²) worst/average, O(n) best
- Space: O(1)
- Stable: Yes
- Adaptive: Yes

#### 2. Selection Sort
- Time: O(n²) all cases
- Space: O(1)
- Stable: No
- Adaptive: No

#### 3. Insertion Sort
- Time: O(n²) worst/average, O(n) best
- Space: O(1)
- Stable: Yes
- Adaptive: Yes

#### 4. Merge Sort
- Time: O(n log n) all cases
- Space: O(n)
- Stable: Yes
- Adaptive: No

#### 5. Quick Sort
- Time: O(n²) worst, O(n log n) average
- Space: O(log n) average
- Stable: No
- Adaptive: No

#### 6. Heap Sort
- Time: O(n log n) all cases
- Space: O(1)
- Stable: No
- Adaptive: No

#### 7. Shell Sort
- Time: Depends on gap sequence
- Space: O(1)
- Stable: No
- Adaptive: Yes

#### 8. Tree Sort
- Time: O(n log n) average, O(n²) worst
- Space: O(n)
- Stable: Depends on implementation

### Non-Comparison Based Sorts

#### 9. Counting Sort
- Time: O(n + k) where k is range
- Space: O(k)
- Stable: Yes
- Works with integers in known range

#### 10. Radix Sort
- Time: O(d × (n + k)) where d is digits
- Space: O(n + k)
- Stable: Yes
- Sorts by individual digits

#### 11. Bucket Sort
- Time: O(n + k) average, O(n²) worst
- Space: O(n × k)
- Stable: Yes
- Distributes elements into buckets

## Searching Algorithms

### 1. Linear Search
- Time: O(n)
- Space: O(1)
- Works on unsorted data

### 2. Binary Search
- Time: O(log n)
- Space: O(1) iterative, O(log n) recursive
- Requires sorted data

### 3. Jump Search
- Time: O(√n)
- Space: O(1)
- Requires sorted data

### 4. Interpolation Search
- Time: O(log log n) average, O(n) worst
- Space: O(1)
- Works well with uniformly distributed data

### 5. Exponential Search
- Time: O(log n)
- Space: O(1)
- Good for unbounded searches

### 6. Ternary Search
- Time: O(log₃ n)
- Space: O(1)
- Divides array into three parts

### 7. Fibonacci Search
- Time: O(log n)
- Space: O(1)
- Uses Fibonacci numbers for division

## Graph Algorithms

### Traversal Algorithms

#### 1. Breadth-First Search (BFS)
- Time: O(V + E)
- Space: O(V)
- Level-order traversal
- Shortest path in unweighted graphs

#### 2. Depth-First Search (DFS)
- Time: O(V + E)
- Space: O(V)
- Explores as far as possible before backtracking
- Topological sorting, cycle detection

### Shortest Path Algorithms

#### 3. Dijkstra's Algorithm
- Time: O((V + E) log V) with min-heap
- Space: O(V)
- Single-source shortest path
- Non-negative weights only

#### 4. Bellman-Ford Algorithm
- Time: O(VE)
- Space: O(V)
- Single-source shortest path
- Handles negative weights
- Detects negative cycles

#### 5. Floyd-Warshall Algorithm
- Time: O(V³)
- Space: O(V²)
- All-pairs shortest path
- Dynamic programming approach

#### 6. Johnson's Algorithm
- Time: O(V² log V + VE)
- Space: O(V²)
- All-pairs shortest path
- Combines Dijkstra and Bellman-Ford

### Minimum Spanning Tree Algorithms

#### 7. Kruskal's Algorithm
- Time: O(E log E)
- Space: O(V)
- Uses Union-Find data structure
- Greedy approach

#### 8. Prim's Algorithm
- Time: O(E log V) with binary heap
- Space: O(V)
- Greedy approach
- Builds tree incrementally

### Other Graph Algorithms

#### 9. Topological Sort
- Time: O(V + E)
- Space: O(V)
- Orders vertices in directed acyclic graph
- Uses DFS or Kahn's algorithm

#### 10. Strongly Connected Components
- **Kosaraju's Algorithm**: O(V + E)
- **Tarjan's Algorithm**: O(V + E)
- Finds SCCs in directed graphs

#### 11. Articulation Points and Bridges
- Time: O(V + E)
- Space: O(V)
- Finds critical vertices/edges
- Uses DFS and low-link values

#### 12. Maximum Flow
- **Ford-Fulkerson**: O(Ef) where f is max flow
- **Edmonds-Karp**: O(VE²)
- **Dinic's Algorithm**: O(V²E)
- **Push-Relabel**: O(V³)

#### 13. Bipartite Matching
- **Hungarian Algorithm**: O(V³)
- **Hopcroft-Karp**: O(E√V)
- Maximum matching in bipartite graphs

## Dynamic Programming Algorithms

### Classic Problems

#### 1. Fibonacci Sequence
- Time: O(n) with memoization
- Space: O(n) or O(1)

#### 2. Longest Common Subsequence (LCS)
- Time: O(mn)
- Space: O(mn) or O(min(m,n))

#### 3. Longest Increasing Subsequence (LIS)
- Time: O(n log n) with binary search
- Space: O(n)

#### 4. Edit Distance (Levenshtein)
- Time: O(mn)
- Space: O(mn) or O(min(m,n))

#### 5. Knapsack Problems
- **0/1 Knapsack**: O(nW) time, O(W) space
- **Unbounded Knapsack**: O(nW) time, O(W) space
- **Fractional Knapsack**: O(n log n) time (greedy)

#### 6. Coin Change Problem
- Time: O(n × amount)
- Space: O(amount)

#### 7. Matrix Chain Multiplication
- Time: O(n³)
- Space: O(n²)

#### 8. Palindrome Partitioning
- Time: O(n³)
- Space: O(n²)

#### 9. Maximum Subarray (Kadane's Algorithm)
- Time: O(n)
- Space: O(1)

#### 10. House Robber Problems
- Time: O(n)
- Space: O(1)

## Greedy Algorithms

### 1. Activity Selection Problem
- Time: O(n log n)
- Select maximum activities without overlap

### 2. Fractional Knapsack
- Time: O(n log n)
- Maximize value with weight constraint

### 3. Huffman Coding
- Time: O(n log n)
- Optimal prefix-free codes

### 4. Job Scheduling
- Various variants with different constraints
- Minimize makespan or maximize profit

### 5. Minimum Number of Coins
- Time: O(n)
- Works with canonical coin systems

## Divide and Conquer Algorithms

### 1. Merge Sort
- Time: O(n log n)
- Stable sorting algorithm

### 2. Quick Sort
- Time: O(n log n) average
- In-place sorting algorithm

### 3. Binary Search
- Time: O(log n)
- Search in sorted array

### 4. Closest Pair of Points
- Time: O(n log n)
- Geometric problem

### 5. Maximum Subarray (Divide & Conquer)
- Time: O(n log n)
- Alternative to Kadane's algorithm

### 6. Strassen's Matrix Multiplication
- Time: O(n^2.807)
- Faster than standard O(n³) approach

### 7. Fast Fourier Transform (FFT)
- Time: O(n log n)
- Signal processing and polynomial multiplication

## Backtracking Algorithms

### 1. N-Queens Problem
- Place N queens on N×N chessboard
- No two queens attack each other

### 2. Sudoku Solver
- Fill 9×9 grid with digits 1-9
- Each row, column, and 3×3 box contains all digits

### 3. Hamiltonian Path/Cycle
- Visit each vertex exactly once
- Path vs cycle (return to start)

### 4. Graph Coloring
- Color vertices with minimum colors
- No adjacent vertices same color

### 5. Subset Sum Problem
- Find subset with given sum
- Decision version of knapsack

### 6. Permutations and Combinations
- Generate all permutations/combinations
- With or without repetition

### 7. Maze Solving
- Find path from start to end
- Rat in maze problem

## String Algorithms

### Pattern Matching

#### 1. Naive String Matching
- Time: O(nm)
- Simple brute force approach

#### 2. KMP (Knuth-Morris-Pratt)
- Time: O(n + m)
- Uses failure function

#### 3. Boyer-Moore Algorithm
- Time: O(n + m) best case
- Bad character and good suffix heuristics

#### 4. Rabin-Karp Algorithm
- Time: O(n + m) average
- Uses rolling hash

#### 5. Z Algorithm
- Time: O(n + m)
- Linear time pattern matching

#### 6. Aho-Corasick Algorithm
- Time: O(n + m + occ)
- Multiple pattern matching

### String Processing

#### 7. Longest Palindromic Substring
- **Manacher's Algorithm**: O(n)
- **Expand Around Centers**: O(n²)

#### 8. String Hashing
- Rolling hash for substring comparisons
- Polynomial hashing

#### 9. Suffix Array Construction
- **Naive**: O(n² log n)
- **DC3 Algorithm**: O(n)
- **SA-IS**: O(n)

#### 10. LCP Array (Longest Common Prefix)
- Time: O(n)
- Used with suffix arrays

## Mathematical Algorithms

### Number Theory

#### 1. Euclidean Algorithm (GCD)
- Time: O(log min(a,b))
- Greatest Common Divisor

#### 2. Extended Euclidean Algorithm
- Time: O(log min(a,b))
- Finds coefficients for Bézout's identity

#### 3. Sieve of Eratosthenes
- Time: O(n log log n)
- Find all primes up to n

#### 4. Modular Exponentiation
- Time: O(log exp)
- Fast power calculation with modulo

#### 5. Chinese Remainder Theorem
- Solve system of congruences
- Number theory applications

#### 6. Fast Multiplication
- **Karatsuba**: O(n^1.585)
- **FFT-based**: O(n log n)

### Matrix Operations

#### 7. Matrix Multiplication
- **Naive**: O(n³)
- **Strassen's**: O(n^2.807)

#### 8. Matrix Exponentiation
- Time: O(n³ log k)
- Fast computation of A^k

#### 9. Gaussian Elimination
- Time: O(n³)
- Solve system of linear equations

### Combinatorics

#### 10. Catalan Numbers
- Various applications in combinatorics
- Dynamic programming computation

#### 11. Binomial Coefficients
- Pascal's triangle
- Combinations calculation

## Computational Geometry Algorithms

### 1. Convex Hull
- **Graham Scan**: O(n log n)
- **Jarvis March**: O(nh)
- **QuickHull**: O(n log n) average

### 2. Line Intersection
- Check if two line segments intersect
- Computational geometry primitive

### 3. Point in Polygon
- **Ray Casting**: O(n)
- **Winding Number**: O(n)

### 4. Closest Pair of Points
- Time: O(n log n)
- Divide and conquer approach

### 5. Rotating Calipers
- Find diameter, width of convex polygon
- Various geometric optimization problems

## Approximation Algorithms

### 1. Vertex Cover
- 2-approximation algorithm
- NP-hard problem

### 2. Traveling Salesman Problem (TSP)
- **Nearest Neighbor**: 2-approximation
- **Christofides**: 1.5-approximation for metric TSP

### 3. Set Cover
- Greedy ln(n)-approximation
- NP-hard problem

### 4. Bin Packing
- **First Fit**: 1.7-approximation
- **Best Fit**: 1.7-approximation
- **First Fit Decreasing**: 11/9-approximation

## Randomized Algorithms

### 1. Randomized QuickSort
- Expected O(n log n) time
- Random pivot selection

### 2. Skip Lists
- Probabilistic data structure
- Expected O(log n) operations

### 3. Miller-Rabin Primality Test
- Probabilistic primality testing
- Polynomial time algorithm

### 4. Monte Carlo Methods
- Random sampling for approximation
- Various applications in optimization

### 5. Las Vegas Algorithms
- Always correct, random runtime
- Randomized algorithms category

## Parallel and Concurrent Algorithms

### 1. Parallel Sorting
- **Parallel Merge Sort**: O(log² n) time
- **Sample Sort**: Distributed sorting

### 2. Parallel Graph Algorithms
- **Parallel BFS**: O(log n) time
- **Parallel Connected Components**

### 3. MapReduce Algorithms
- Distributed computing paradigm
- Large-scale data processing

### 4. Lock-free Data Structures
- Concurrent programming
- Avoid blocking synchronization

## Cache-Oblivious Algorithms

### 1. Cache-Oblivious Sorting
- Optimal cache performance
- Independent of cache parameters

### 2. Cache-Oblivious Matrix Multiplication
- Recursive divide and conquer
- Optimal cache complexity

### 3. Van Emde Boas Tree
- O(log log u) operations
- Predecessor/successor queries

This comprehensive reference covers the major data structures and algorithms used in computer science and software engineering. Each entry includes key features, time/space complexities, and primary use cases.
