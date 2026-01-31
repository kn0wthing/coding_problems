## 1. Sliding Window (18 problems)

This topic has distinct sub-patterns that each need practice.

### Fixed Window
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Maximum Average Subarray I (643) | Basic fixed window |
| 2 | Sliding Window Maximum (239) | Fixed window + monotonic deque |
| 3 | Sliding Window Median (480) | Fixed window + two heaps + lazy deletion |

### Variable Window — Shrink When Invalid
| # | Problem | Key Learning |
|---|---------|--------------|
| 4 | Longest Substring Without Repeating Characters (3) | Basic variable window |
| 5 | Longest Repeating Character Replacement (424) | Window with frequency constraint |
| 6 | Max Consecutive Ones III (1004) | Binary array window |
| 7 | Fruit Into Baskets (904) | At most k distinct |
| 8 | Longest Substring with At Most K Distinct Characters (340) | Generalized k distinct |
| 9 | Get Equal Substrings Within Budget (1208) | Cost-based window |

### Variable Window — Shrink When Valid (Minimum)
| # | Problem | Key Learning |
|---|---------|--------------|
| 10 | Minimum Window Substring (76) | The hardest standard template |
| 11 | Minimum Size Subarray Sum (209) | Minimum length with sum |
| 12 | Minimum Window Subsequence (727) | Subsequence matching |

### Count Subarrays — atMost(k) Trick
| # | Problem | Key Learning |
|---|---------|--------------|
| 13 | Subarrays with K Different Integers (992) | exactly(k) = atMost(k) - atMost(k-1) |
| 14 | Count Number of Nice Subarrays (1248) | Same trick on odd numbers |
| 15 | Binary Subarrays With Sum (930) | Same trick on binary |
| 16 | Number of Substrings Containing All Three Characters (1358) | atLeast variation |

### Advanced / Hybrid
| # | Problem | Key Learning |
|---|---------|--------------|
| 17 | Minimum Number of K Consecutive Bit Flips (995) | Window + greedy + state tracking |
| 18 | Shortest Subarray with Sum at Least K (862) | Window fails (negatives), need monotonic deque |

---



## Sliding Window — Additional Variations

### Sliding Window with Data Structures
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Longest Continuous Subarray With Absolute Diff <= Limit (1438) | Two deques (min and max) |
| 2 | Max Value of Equation (1499) | Monotonic deque in window |
| 3 | Constrained Subsequence Sum (1425) | DP + monotonic deque |
| 4 | Jump Game VI (1696) | DP + monotonic deque |

### Sliding Window with Multiple Conditions
| # | Problem | Key Learning |
|---|---------|--------------|
| 5 | Count Subarrays With Fixed Bounds (2444) | Track both min and max positions |
| 6 | Longest Substring with At Least K Repeating Characters (395) | Divide and conquer OR enumerate unique chars |
| 7 | Maximum Number of Visible Points (1610) | Circular angle-based window |

### Sliding Window on Complement / Reverse Thinking
| # | Problem | Key Learning |
|---|---------|--------------|
| 8 | Minimum Operations to Reduce X to Zero (1658) | Find longest middle with sum = total - x |
| 9 | Maximum Points You Can Obtain from Cards (1423) | Window on complement |
| 10 | Minimum Swaps to Group All 1's Together II (2134) | Circular array window |

### Fixed Window Variations
| # | Problem | Key Learning |
|---|---------|--------------|
| 11 | Grumpy Bookstore Owner (1052) | Maximize gain in fixed window |
| 12 | K Radius Subarray Averages (2090) | Fixed window with edge handling |
| 13 | Find All Anagrams in String (438) | Fixed window frequency match |
| 14 | Permutation in String (567) | Fixed window existence |

### Multi-Window / Complex Counting
| # | Problem | Key Learning |
|---|---------|--------------|
| 15 | Count Subarrays Where Max Element Appears at Least K Times (2962) | Contribution with window |
| 16 | Shortest Subarray to be Removed to Make Array Sorted (1574) | Two pointers from ends |
| 17 | Maximum Fruits Harvested After at Most K Steps (2106) | Prefix sum + window |
| 18 | Minimum Adjacent Swaps for K Consecutive Ones (1703) | Median + window |

---

## 2. Two Pointers (14 problems)

### Opposite Ends
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Two Sum II (167) | Basic converging pointers |
| 2 | 3Sum (15) | Fix one + two pointer + skip duplicates |
| 3 | 4Sum (18) | Fix two + two pointer |
| 4 | 3Sum Closest (16) | Optimization variant |
| 5 | Container With Most Water (11) | Greedy movement proof |
| 6 | Trapping Rain Water (42) | Two pointer O(1) space solution |

### Same Direction (Slow/Fast)
| # | Problem | Key Learning |
|---|---------|--------------|
| 7 | Remove Duplicates from Sorted Array II (80) | In-place with constraint |
| 8 | Move Zeroes (283) | Partition style |
| 9 | Sort Colors (75) | Dutch national flag, 3-way partition |

### Two Arrays
| # | Problem | Key Learning |
|---|---------|--------------|
| 10 | Merge Sorted Array (88) | Merge from end |
| 11 | Interval List Intersections (986) | Two lists intersection |
| 12 | Shortest Word Distance III (245) | Handle same word |

### Advanced
| # | Problem | Key Learning |
|---|---------|--------------|
| 13 | 4Sum II (454) | Hashmap meets pair thinking |
| 14 | Boats to Save People (881) | Greedy pairing |

---

## 3. Monotonic Stack (16 problems)

### Next/Previous Greater/Smaller
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Next Greater Element I (496) | Basic template |
| 2 | Next Greater Element II (503) | Circular array |
| 3 | Daily Temperatures (739) | Next greater index |
| 4 | Online Stock Span (901) | Previous greater/equal span |
| 5 | 132 Pattern (456) | Track max on right |

### Histogram Pattern
| # | Problem | Key Learning |
|---|---------|--------------|
| 6 | Largest Rectangle in Histogram (84) | THE classic |
| 7 | Maximal Rectangle (85) | Apply histogram per row |
| 8 | Trapping Rain Water (42) | Stack solution |

### Contribution Technique
| # | Problem | Key Learning |
|---|---------|--------------|
| 9 | Sum of Subarray Minimums (907) | Count contribution of each element |
| 10 | Sum of Subarray Ranges (2104) | Max contribution - min contribution |
| 11 | Sum of Total Strength of Wizards (2281) | Contribution + prefix of prefix |

### String / Number Construction
| # | Problem | Key Learning |
|---|---------|--------------|
| 12 | Remove K Digits (402) | Build smallest number |
| 13 | Remove Duplicate Letters (316) | Lexicographically smallest |
| 14 | Create Maximum Number (321) | Two arrays, merge |

### Advanced
| # | Problem | Key Learning |
|---|---------|--------------|
| 15 | Maximum Width Ramp (962) | Monotonic + binary search |
| 16 | Odd Even Jump (975) | Monotonic + DP |

---

## Monotonic Stack/Deque — Additional Variations

### Double Deque Pattern
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Longest Continuous Subarray With Absolute Diff <= Limit (1438) | Min deque + max deque simultaneously |
| 2 | Shortest Subarray with Sum at Least K (862) | Monotonic deque (not two, but essential) |

### Monotonic Deque + DP
| # | Problem | Key Learning |
|---|---------|--------------|
| 3 | Constrained Subsequence Sum (1425) | DP transition with deque optimization |
| 4 | Jump Game VI (1696) | Max in sliding window for DP |
| 5 | Max Value of Equation (1499) | Deque maintains y - x values |
| 6 | Maximum Number of Books You Can Take (2355) | Stack + arithmetic progression DP |

### Stack with Complex State
| # | Problem | Key Learning |
|---|---------|--------------|
| 7 | Number of Visible People in a Queue (1944) | Stack counting visible |
| 8 | Steps to Make Array Non-decreasing (2289) | Reverse simulation with stack |
| 9 | Robot Collisions (2751) | Stack with collision physics |
| 10 | Find Building Where Alice and Bob Can Meet (2940) | Offline + monotonic stack |
| 11 | Number of People That Can Be Seen in a Grid (2282) | 2D visibility |

### Stack + Contribution (Advanced)
| # | Problem | Key Learning |
|---|---------|--------------|
| 12 | Sum of Total Strength of Wizards (2281) | Prefix of prefix sum + stack |
| 13 | Count Submatrices With All Ones (1504) | Stack per row |
| 14 | Maximum Score of a Good Subarray (1793) | Expand from k with stack |
| 15 | Maximal Rectangle (85) | Already have, but critical |

### Stack for Parsing / Expression
| # | Problem | Key Learning |
|---|---------|--------------|
| 16 | Basic Calculator (224) | Stack for parentheses |
| 17 | Basic Calculator II (227) | Operator precedence |
| 18 | Basic Calculator III (772) | Combined |
| 19 | Number of Atoms (726) | Nested parsing |
| 20 | Decode String (394) | Nested brackets |
| 21 | Exclusive Time of Functions (636) | Call stack simulation |

---

## 4. Binary Search (20 problems)

### Standard Binary Search
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Search Insert Position (35) | Lower bound |
| 2 | Find First and Last Position (34) | Lower + upper bound |
| 3 | Search a 2D Matrix (74) | Flatten to 1D |
| 4 | Search a 2D Matrix II (240) | Staircase search |

### Rotated Array
| # | Problem | Key Learning |
|---|---------|--------------|
| 5 | Search in Rotated Sorted Array (33) | Find sorted half |
| 6 | Search in Rotated Sorted Array II (81) | With duplicates |
| 7 | Find Minimum in Rotated Sorted Array (153) | Find pivot |
| 8 | Find Minimum in Rotated Sorted Array II (154) | With duplicates |

### Binary Search on Answer
| # | Problem | Key Learning |
|---|---------|--------------|
| 9 | Koko Eating Bananas (875) | Minimize maximum rate |
| 10 | Capacity To Ship Packages (1011) | Minimize maximum capacity |
| 11 | Split Array Largest Sum (410) | Minimize maximum sum |
| 12 | Magnetic Force Between Two Balls (1552) | Maximize minimum distance |
| 13 | Minimized Maximum of Products (2064) | Minimize maximum |
| 14 | Minimum Time to Complete Trips (2187) | Time-based feasibility |
| 15 | Minimum Speed to Arrive on Time (1870) | Floating point binary search |

### Kth Element
| # | Problem | Key Learning |
|---|---------|--------------|
| 16 | Kth Smallest Element in a Sorted Matrix (378) | BS + counting |
| 17 | Find K-th Smallest Pair Distance (719) | BS + two pointer count |
| 18 | Kth Smallest Number in Multiplication Table (668) | BS + counting |

### Advanced
| # | Problem | Key Learning |
|---|---------|--------------|
| 19 | Median of Two Sorted Arrays (4) | Partition based BS |
| 20 | Find in Mountain Array (1095) | Find peak + two BS |

---

## Binary Search — Additional Variations

### Binary Search + Complex Feasibility Check
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Maximum Number of Tasks You Can Assign (2071) | Binary search + greedy + deque |
| 2 | Minimum Time to Repair Cars (2594) | Multi-worker feasibility |
| 3 | Maximum Running Time of N Computers (2141) | Sum-based feasibility |
| 4 | Maximum Candies Allocated to K Children (2226) | Simple but good practice |
| 5 | Cutting Ribbons (1891) | Maximize minimum |
| 6 | Minimum Number of Days to Make m Bouquets (1482) | Consecutive constraint |

### Binary Search + Data Structure
| # | Problem | Key Learning |
|---|---------|--------------|
| 7 | Count of Range Sum (327) | Binary search in merge sort or BIT |
| 8 | Longest Increasing Subsequence (300) | Binary search for O(n log n) |
| 9 | Russian Doll Envelopes (354) | Sort + LIS with binary search |
| 10 | Find Right Interval (436) | Binary search on sorted intervals |

### Binary Search on Strings
| # | Problem | Key Learning |
|---|---------|--------------|
| 11 | Search Suggestions System (1268) | Binary search + trie hybrid |
| 12 | Longest Duplicate Substring (1044) | Binary search + rolling hash |
| 13 | Maximum Number of Removable Characters (1898) | Binary search on removals |

### Interactive / Online Binary Search
| # | Problem | Key Learning |
|---|---------|--------------|
| 14 | Guess Number Higher or Lower (374) | Basic interactive |
| 15 | Find in Mountain Array (1095) | API-based search |
| 16 | First Bad Version (278) | Minimize API calls |

### Binary Search with Prefix Sum
| # | Problem | Key Learning |
|---|---------|--------------|
| 17 | Random Pick with Weight (528) | Weighted random via prefix + BS |
| 18 | Find the Longest Substring Containing Vowels in Even Counts (1371) | Bitmask + first occurrence |
| 19 | Maximum Sum of 3 Non-Overlapping Subarrays (689) | Prefix + DP + BS reconstruction |

### Binary Search Edge Cases
| # | Problem | Key Learning |
|---|---------|--------------|
| 20 | H-Index II (275) | Tricky condition |
| 21 | Kth Missing Positive Number (1539) | Missing count calculation |
| 22 | Sum of Mutated Array Closest to Target (1300) | Minimize absolute difference |
| 23 | Minimum Speed to Arrive on Time (1870) | Floating point precision |

---

## 5. Linked List (15 problems)

### Reversal
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Reverse Linked List (206) | Iterative + recursive |
| 2 | Reverse Linked List II (92) | Reverse portion |
| 3 | Reverse Nodes in k-Group (25) | Full mastery of reversal |
| 4 | Swap Nodes in Pairs (24) | Pair reversal |

### Two Pointers / Cycle
| # | Problem | Key Learning |
|---|---------|--------------|
| 5 | Linked List Cycle II (142) | Floyd's with entry point |
| 6 | Find the Duplicate Number (287) | Floyd's on array |
| 7 | Intersection of Two Linked Lists (160) | Length difference or two pass |
| 8 | Remove Nth Node From End (19) | Two pointer gap |
| 9 | Reorder List (143) | Find middle + reverse + merge |

### Merge / Sort
| # | Problem | Key Learning |
|---|---------|--------------|
| 10 | Merge Two Sorted Lists (21) | Basic merge |
| 11 | Merge k Sorted Lists (23) | Heap or divide conquer |
| 12 | Sort List (148) | Merge sort on linked list |

### Complex Manipulation
| # | Problem | Key Learning |
|---|---------|--------------|
| 13 | Copy List with Random Pointer (138) | Clone with interleaving |
| 14 | LRU Cache (146) | Doubly linked list + hashmap |
| 15 | LFU Cache (460) | Multiple lists + hashmap |

---

## 6. Trees — Traversal & Construction (18 problems)

### Basic Traversal
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Binary Tree Inorder Traversal (94) | Iterative with stack |
| 2 | Binary Tree Level Order Traversal (102) | BFS template |
| 3 | Binary Tree Zigzag Level Order (103) | Level order variation |
| 4 | Vertical Order Traversal (987) | Coordinate system + sorting |
| 5 | Boundary of Binary Tree (545) | Multiple traversals combined |

### Construction
| # | Problem | Key Learning |
|---|---------|--------------|
| 6 | Construct Binary Tree from Preorder and Inorder (105) | Classic construction |
| 7 | Construct Binary Tree from Inorder and Postorder (106) | Variation |
| 8 | Construct Binary Tree from Preorder and Postorder (889) | Without inorder |
| 9 | Serialize and Deserialize Binary Tree (297) | Full serialization |
| 10 | Serialize and Deserialize BST (449) | BST-specific optimization |

### Morris Traversal
| # | Problem | Key Learning |
|---|---------|--------------|
| 11 | Recover Binary Search Tree (99) | Morris for O(1) space |
| 12 | Binary Tree Inorder Morris | Know the technique |

### Path Problems
| # | Problem | Key Learning |
|---|---------|--------------|
| 13 | Binary Tree Maximum Path Sum (124) | Global vs local return |
| 14 | Path Sum III (437) | Prefix sum on tree |
| 15 | Longest Univalue Path (687) | Path through node |
| 16 | Diameter of Binary Tree (543) | Simpler version of 124 |

### Advanced Structure
| # | Problem | Key Learning |
|---|---------|--------------|
| 17 | Populating Next Right Pointers II (117) | Level linking O(1) space |
| 18 | Flatten Binary Tree to Linked List (114) | In-place restructure |

---

## 7. Trees — BST Specific (10 problems)

| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Validate Binary Search Tree (98) | Range validation |
| 2 | Kth Smallest Element in BST (230) | Inorder property |
| 3 | Inorder Successor in BST (285) | Parent pointer or search |
| 4 | Inorder Successor in BST II (510) | With parent pointer |
| 5 | Lowest Common Ancestor of BST (235) | BST-specific LCA |
| 6 | Delete Node in a BST (450) | All deletion cases |
| 7 | Convert BST to Greater Tree (538) | Reverse inorder |
| 8 | Closest Binary Search Tree Value II (272) | K closest values |
| 9 | Count of Smaller Numbers After Self (315) | BST or BIT |
| 10 | Convert Sorted List to BST (109) | Balanced construction |

---

## 8. Trees — LCA & Ancestors (8 problems)

| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Lowest Common Ancestor of Binary Tree (236) | Standard DFS |
| 2 | Lowest Common Ancestor of BST (235) | BST optimization |
| 3 | Lowest Common Ancestor III (1650) | Nodes might not exist |
| 4 | Lowest Common Ancestor IV (1676) | Multiple nodes |
| 5 | Lowest Common Ancestor of Deepest Leaves (1123) | Depth tracking |
| 6 | Kth Ancestor of a Tree Node (1483) | Binary lifting |
| 7 | Maximum Difference Between Node and Ancestor (1026) | Track min/max |
| 8 | LCA with Parent Pointers | Two pointer technique |

---

## 9. Trees — DP on Trees (12 problems)

| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | House Robber III (337) | Rob/not rob state |
| 2 | Binary Tree Cameras (968) | 3 states: covered, has camera, not covered |
| 3 | Distribute Coins in Binary Tree (979) | Flow calculation |
| 4 | Sum of Distances in Tree (834) | Rerooting technique |
| 5 | Longest Path With Different Adjacent Characters (2246) | Tree DP + state |
| 6 | Maximum Product of Splitted Binary Tree (1339) | Total sum - subtree sum |
| 7 | Linked List in Binary Tree (1367) | DP + DFS |
| 8 | Count Good Nodes in Binary Tree (1448) | Track max in path |
| 9 | Delete Nodes And Return Forest (1110) | Deletion + root tracking |
| 10 | All Possible Full Binary Trees (894) | Memoized construction |
| 11 | Unique Binary Search Trees II (95) | Generate all BSTs |
| 12 | Binary Tree Coloring Game (1145) | Component size analysis |

---

## 10. Graphs — BFS (16 problems)

### Basic BFS
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Number of Islands (200) | Grid BFS template |
| 2 | Rotting Oranges (994) | Multi-source BFS |
| 3 | 01 Matrix (542) | Multi-source from targets |
| 4 | Walls and Gates (286) | Multi-source, fill distances |

### Shortest Path Unweighted
| # | Problem | Key Learning |
|---|---------|--------------|
| 5 | Word Ladder (127) | State transformation BFS |
| 6 | Word Ladder II (126) | BFS + backtrack for all paths |
| 7 | Minimum Knight Moves (1197) | Infinite grid BFS |
| 8 | Shortest Path in Binary Matrix (1091) | 8-directional |
| 9 | Shortest Path to Get All Keys (864) | BFS + bitmask state |

### 0-1 BFS
| # | Problem | Key Learning |
|---|---------|--------------|
| 10 | Minimum Cost to Make at Least One Valid Path (1368) | 0-1 BFS with deque |
| 11 | Minimum Obstacle Removal (2290) | 0-1 BFS |

### Multi-state BFS
| # | Problem | Key Learning |
|---|---------|--------------|
| 12 | Shortest Path Visiting All Nodes (847) | BFS + bitmask |
| 13 | Sliding Puzzle (773) | State as string BFS |
| 14 | Open the Lock (752) | State transformation |

### Advanced BFS
| # | Problem | Key Learning |
|---|---------|--------------|
| 15 | Bus Routes (815) | BFS on routes not stops |
| 16 | Jump Game IV (1345) | BFS with pruning |

---

## 11. Graphs — DFS (14 problems)

### Grid DFS
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Pacific Atlantic Water Flow (417) | Reverse DFS from edges |
| 2 | Surrounded Regions (130) | Border-connected components |
| 3 | Making A Large Island (827) | Label components + simulate |
| 4 | Longest Increasing Path in Matrix (329) | DFS + memoization |
| 5 | Number of Distinct Islands (694) | Serialize island shape |

### Cycle Detection
| # | Problem | Key Learning |
|---|---------|--------------|
| 6 | Course Schedule (207) | Cycle in directed graph |
| 7 | Course Schedule II (210) | Topological order |
| 8 | Detect Cycles in 2D Grid (1559) | Grid cycle detection |

### DFS with State
| # | Problem | Key Learning |
|---|---------|--------------|
| 9 | All Paths From Source to Target (797) | Path enumeration |
| 10 | Clone Graph (133) | DFS with visited map |
| 11 | Evaluate Division (399) | Graph as division relationships |
| 12 | Reconstruct Itinerary (332) | Eulerian path |

### Advanced DFS
| # | Problem | Key Learning |
|---|---------|--------------|
| 13 | Redundant Connection (684) | Find cycle edge |
| 14 | Redundant Connection II (685) | Directed graph, multiple cases |

---

## 12. Graphs — Topological Sort (10 problems)

| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Course Schedule (207) | Basic cycle detection |
| 2 | Course Schedule II (210) | Return the order |
| 3 | Alien Dictionary (269) | Build graph from constraints |
| 4 | Sequence Reconstruction (444) | Unique topological order |
| 5 | Parallel Courses (1136) | Maximum depth |
| 6 | Parallel Courses II (1494) | Topo sort + bitmask DP |
| 7 | Parallel Courses III (2050) | Time to complete with dependencies |
| 8 | Minimum Height Trees (310) | Centroid finding via topo peel |
| 9 | Sort Items by Groups (1203) | Two-level topo sort |
| 10 | Build a Matrix With Conditions (2392) | Independent row/col topo sorts |

---

## 13. Graphs — Shortest Path (12 problems)

### Dijkstra
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Network Delay Time (743) | Classic Dijkstra |
| 2 | Path with Maximum Probability (1514) | Max probability (max heap) |
| 3 | Path With Minimum Effort (1631) | Minimize max edge |
| 4 | Swim in Rising Water (778) | Binary search + BFS or Dijkstra |
| 5 | Minimum Cost to Reach Destination in Time (1928) | Dijkstra with constraint |

### Bellman-Ford
| # | Problem | Key Learning |
|---|---------|--------------|
| 6 | Cheapest Flights Within K Stops (787) | BF with k iterations |
| 7 | Negative Weight Cycle Detection | Know when to use |

### Floyd-Warshall
| # | Problem | Key Learning |
|---|---------|--------------|
| 8 | Find the City (1334) | All pairs shortest path |
| 9 | Course Schedule IV (1462) | Transitive closure |

### Advanced
| # | Problem | Key Learning |
|---|---------|--------------|
| 10 | Shortest Path with Alternating Colors (1129) | Multi-state Dijkstra |
| 11 | Number of Ways to Arrive at Destination (1976) | Dijkstra + count paths |
| 12 | Second Minimum Time to Reach Destination (2045) | Track two best times |

---

## 14. Graphs — Union Find (12 problems)

### Basic Operations
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Number of Provinces (547) | Basic union find |
| 2 | Number of Connected Components (323) | Count components |
| 3 | Redundant Connection (684) | Find cycle-causing edge |

### Union Find with Data
| # | Problem | Key Learning |
|---|---------|--------------|
| 4 | Accounts Merge (721) | Track data per component |
| 5 | Smallest String With Swaps (1202) | Sort within components |
| 6 | Evaluate Division (399) | Weighted union find |

### Dynamic Connectivity
| # | Problem | Key Learning |
|---|---------|--------------|
| 7 | Number of Operations to Make Network Connected (1319) | Count components + edges |
| 8 | Satisfiability of Equality Equations (990) | Union + verify |
| 9 | Graph Connectivity With Threshold (1627) | Factor-based union |

### Advanced
| # | Problem | Key Learning |
|---|---------|--------------|
| 10 | Swim in Rising Water (778) | Union find solution |
| 11 | Checking Existence of Edge Length Limited Paths (1697) | Offline + sort + union find |
| 12 | Making A Large Island (827) | Union find solution |

---

## Union Find — Comprehensive Deep Dive

### Grid-Based Union Find
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Number of Islands II (305) | Dynamic island creation |
| 2 | Regions Cut By Slashes (959) | Scale up grid 3x, creative mapping |
| 3 | Most Stones Removed with Same Row or Column (947) | Row/column as virtual nodes |
| 4 | Making A Large Island (827) | Label + simulate flip |
| 5 | Bricks Falling When Hit (803) | **Reverse time** union find |

### Factor/Math Based Union Find
| # | Problem | Key Learning |
|---|---------|--------------|
| 6 | Largest Component Size by Common Factor (952) | Union by prime factors |
| 7 | Gcd Sort of an Array (1998) | Union if GCD > 1 |
| 8 | Graph Connectivity With Threshold (1627) | Union multiples |

### String Union Find
| # | Problem | Key Learning |
|---|---------|--------------|
| 9 | Lexicographically Smallest Equivalent String (1061) | Track min char per component |
| 10 | Similar String Groups (839) | Union similar strings |
| 11 | Groups of Strings (2157) | Edit distance 1 grouping |

### Union Find with Weights/Ratios
| # | Problem | Key Learning |
|---|---------|--------------|
| 12 | Evaluate Division (399) | Weighted edges in union find |
| 13 | Rank Transform of a Matrix (1632) | Union find + greedy ranking |

### Reverse Time Union Find
| # | Problem | Key Learning |
|---|---------|--------------|
| 14 | Bricks Falling When Hit (803) | Process removals in reverse |
| 15 | Minimize Malware Spread (924) | Try removing each node |
| 16 | Minimize Malware Spread II (928) | Variation |

### Union Find with Constraints
| # | Problem | Key Learning |
|---|---------|--------------|
| 17 | Process Restricted Friend Requests (2076) | Check before union |
| 18 | Couples Holding Hands (765) | Cycle counting |
| 19 | Minimize Hamming Distance After Swap Operations (1722) | Frequency per component |

### Advanced Union Find
| # | Problem | Key Learning |
|---|---------|--------------|
| 20 | Remove Max Number of Edges to Keep Graph Fully Traversable (1579) | Two union finds (Alice/Bob) |
| 21 | Checking Existence of Edge Length Limited Paths (1697) | Offline + sorted queries |
| 22 | Checking Existence of Edge Length Limited Paths II (1724) | Online with persistent UF |
| 23 | Number of Good Paths (2421) | Process nodes in sorted value order |
| 24 | Count Unreachable Pairs of Nodes (2316) | Component size multiplication |

---

## 15. Graphs — Advanced Algorithms (10 problems)

### Tarjan's Algorithm
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Critical Connections in a Network (1192) | Find bridges |
| 2 | Articulation Points | Find cut vertices |
| 3 | Strongly Connected Components | Tarjan's SCC |

### MST (Minimum Spanning Tree)
| # | Problem | Key Learning |
|---|---------|--------------|
| 4 | Min Cost to Connect All Points (1584) | Prim or Kruskal |
| 5 | Connecting Cities With Minimum Cost (1135) | MST application |
| 6 | Find Critical and Pseudo-Critical Edges (1489) | MST + edge analysis |

### Bipartite
| # | Problem | Key Learning |
|---|---------|--------------|
| 7 | Is Graph Bipartite (785) | Two coloring |
| 8 | Possible Bipartition (886) | Bipartite with dislikes |

### Eulerian Path
| # | Problem | Key Learning |
|---|---------|--------------|
| 9 | Reconstruct Itinerary (332) | Hierholzer's algorithm |
| 10 | Valid Arrangement of Pairs (2097) | Eulerian path on directed |

---

## Graphs — Additional Missing Topics

### Bidirectional BFS
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Word Ladder (127) | Meet in middle optimization |
| 2 | Minimum Genetic Mutation (433) | Small state space |
| 3 | Open the Lock (752) | Bidirectional from start and target |

### 0-1 BFS (Deque-based)
| # | Problem | Key Learning |
|---|---------|--------------|
| 4 | Minimum Cost to Make at Least One Valid Path (1368) | 0 cost = front, 1 cost = back |
| 5 | Minimum Obstacle Removal to Reach Corner (2290) | Same pattern |
| 6 | Minimum Cost to Reach Destination in Time (1928) | BFS with pruning |

### BFS with Complex State
| # | Problem | Key Learning |
|---|---------|--------------|
| 7 | Shortest Path in a Grid with Obstacles Elimination (1293) | State = (x, y, k remaining) |
| 8 | Escape the Spreading Fire (2258) | Binary search + multi-source BFS |
| 9 | Minimum Moves to Reach Target with Rotations (1210) | Snake rotation state |
| 10 | Minimum Time to Visit a Cell In a Grid (2577) | Dijkstra with parity |

### Tree Algorithms
| # | Problem | Key Learning |
|---|---------|--------------|
| 11 | Tree Diameter (1245) | Two BFS or DP |
| 12 | Find Distance in a Binary Tree (1740) | LCA application |
| 13 | Height of Binary Tree After Subtree Removal Queries (2458) | Precompute left/right max depths |
| 14 | Minimum Edge Weight Equilibrium Queries (2846) | LCA + frequency tracking |
| 15 | Difference Between Maximum and Minimum Price Sum (2538) | Rerooting DP |

### Game Theory on Graphs
| # | Problem | Key Learning |
|---|---------|--------------|
| 16 | Cat and Mouse (913) | BFS from terminal states |
| 17 | Cat and Mouse II (1728) | State space game |

### Multi-Source/Sink Problems
| # | Problem | Key Learning |
|---|---------|--------------|
| 18 | Minimum Weighted Subgraph With Required Paths (2203) | Meet in middle on graphs |
| 19 | Reachable Nodes In Subdivided Graph (882) | Dijkstra with fractional edges |

### Strongly Connected Components
| # | Problem | Key Learning |
|---|---------|--------------|
| 20 | Minimum Number of Days to Disconnect Island (1568) | Articulation point concept |
| 21 | Critical Connections in a Network (1192) | Already have, but essential |

---

## 16. Backtracking (16 problems)

### Permutations & Combinations
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Permutations (46) | Basic permutation |
| 2 | Permutations II (47) | With duplicates |
| 3 | Combinations (77) | Basic combination |
| 4 | Combination Sum (39) | Unlimited use |
| 5 | Combination Sum II (40) | Each once, with duplicates |
| 6 | Combination Sum III (216) | Fixed count, fixed range |
| 7 | Subsets (78) | All subsets |
| 8 | Subsets II (90) | With duplicates |

### Partitioning
| # | Problem | Key Learning |
|---|---------|--------------|
| 9 | Palindrome Partitioning (131) | Partition into palindromes |
| 10 | Restore IP Addresses (93) | Partition with constraints |
| 11 | Partition to K Equal Sum Subsets (698) | K-way partition |

### Constraint Satisfaction
| # | Problem | Key Learning |
|---|---------|--------------|
| 12 | N-Queens (51) | Classic CSP |
| 13 | N-Queens II (52) | Count solutions |
| 14 | Sudoku Solver (37) | Heavy pruning |
| 15 | Word Search II (212) | Trie + backtracking |
| 16 | Expression Add Operators (282) | Arithmetic backtracking |

---

## 17. DP — Linear (18 problems)

### Basic Linear
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | House Robber (198) | Take/skip pattern |
| 2 | House Robber II (213) | Circular array |
| 3 | Delete and Earn (740) | Reduce to house robber |
| 4 | Maximum Subarray (53) | Kadane's algorithm |
| 5 | Maximum Product Subarray (152) | Track min and max |
| 6 | Best Time to Buy and Sell Stock (121) | Track minimum |

### Subsequence
| # | Problem | Key Learning |
|---|---------|--------------|
| 7 | Longest Increasing Subsequence (300) | O(n²) and O(n log n) |
| 8 | Number of Longest Increasing Subsequence (673) | Count LIS |
| 9 | Longest Arithmetic Subsequence (1027) | DP with hashmap |
| 10 | Longest Arithmetic Subsequence of Given Difference (1218) | Hashmap optimization |
| 11 | Russian Doll Envelopes (354) | 2D LIS |

### String Linear
| # | Problem | Key Learning |
|---|---------|--------------|
| 12 | Decode Ways (91) | Counting paths |
| 13 | Decode Ways II (639) | With wildcards |
| 14 | Word Break (139) | Can segment |
| 15 | Word Break II (140) | All segmentations |
| 16 | Longest Valid Parentheses (32) | Stack or DP |

### Advanced Linear
| # | Problem | Key Learning |
|---|---------|--------------|
| 17 | Maximum Sum Circular Subarray (918) | Kadane variant |
| 18 | Best Sightseeing Pair (1014) | Decompose optimization |

---

## 18. DP — Knapsack (15 problems)

### 0/1 Knapsack
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Partition Equal Subset Sum (416) | Classic 0/1 |
| 2 | Target Sum (494) | Count ways to reach target |
| 3 | Last Stone Weight II (1049) | Minimize difference |
| 4 | Ones and Zeroes (474) | 2D capacity |

### Unbounded Knapsack
| # | Problem | Key Learning |
|---|---------|--------------|
| 5 | Coin Change (322) | Minimum coins |
| 6 | Coin Change 2 (518) | Count combinations |
| 7 | Perfect Squares (279) | Minimum squares |
| 8 | Integer Break (343) | Maximize product |

### Bounded Knapsack
| # | Problem | Key Learning |
|---|---------|--------------|
| 9 | Combination Sum IV (377) | Permutations count |
| 10 | Minimum Cost For Tickets (983) | Time-based knapsack |

### Multi-dimensional
| # | Problem | Key Learning |
|---|---------|--------------|
| 11 | Profitable Schemes (879) | 3D: people, profit, crimes |
| 12 | Tallest Billboard (956) | Difference as state |
| 13 | Number of Ways to Earn Points (2585) | 2D with constraints |

### Advanced
| # | Problem | Key Learning |
|---|---------|--------------|
| 14 | Maximum Value of K Coins From Piles (2218) | Piles as items |
| 15 | Number of Ways to Form a Target String (1639) | Position + character |

---

## 19. DP — Two Sequences (12 problems)

### LCS Family
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Longest Common Subsequence (1143) | Classic LCS |
| 2 | Longest Common Substring | Variation (not on LC) |
| 3 | Shortest Common Supersequence (1092) | LCS + reconstruction |
| 4 | Delete Operation for Two Strings (583) | Min deletions via LCS |
| 5 | Minimum ASCII Delete Sum (712) | LCS with weights |
| 6 | Max Dot Product of Two Subsequences (1458) | LCS structure, different relation |

### Edit Distance Family
| # | Problem | Key Learning |
|---|---------|--------------|
| 7 | Edit Distance (72) | Classic |
| 8 | One Edit Distance (161) | O(n) check |
| 9 | Distinct Subsequences (115) | Count ways |

### Matching
| # | Problem | Key Learning |
|---|---------|--------------|
| 10 | Wildcard Matching (44) | * and ? matching |
| 11 | Regular Expression Matching (10) | * means zero or more of preceding |
| 12 | Interleaving String (97) | Two strings merge |

---

## 20. DP — Interval (12 problems)

### Basic Interval
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Longest Palindromic Subsequence (516) | Classic interval |
| 2 | Longest Palindromic Substring (5) | Expand or DP |
| 3 | Palindromic Substrings (647) | Count all |
| 4 | Palindrome Partitioning II (132) | Minimum cuts |

### Matrix Chain Style
| # | Problem | Key Learning |
|---|---------|--------------|
| 5 | Burst Balloons (312) | Add boundary trick |
| 6 | Minimum Cost to Merge Stones (1000) | Merge with constraint |
| 7 | Minimum Score Triangulation (1039) | Polygon triangulation |

### Advanced Interval
| # | Problem | Key Learning |
|---|---------|--------------|
| 8 | Strange Printer (664) | Print optimization |
| 9 | Remove Boxes (546) | 3D interval DP |
| 10 | Minimum Cost Tree From Leaf Values (1130) | Stack or interval DP |
| 11 | Minimum Insertion Steps to Make Palindrome (1312) | Related to LPS |
| 12 | Stone Game III (1406) | Game theory interval |

---

## 21. DP — State Machine (14 problems)

### Stock Problems
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Best Time to Buy and Sell Stock II (122) | Unlimited transactions |
| 2 | Best Time to Buy and Sell Stock III (123) | At most 2 transactions |
| 3 | Best Time to Buy and Sell Stock IV (188) | At most k transactions |
| 4 | Best Time to Buy and Sell Stock with Cooldown (309) | State: hold, sold, cooldown |
| 5 | Best Time to Buy and Sell Stock with Transaction Fee (714) | Fee per transaction |

### Paint/Color Problems
| # | Problem | Key Learning |
|---|---------|--------------|
| 6 | Paint House (256) | 3 colors, adjacent different |
| 7 | Paint House II (265) | K colors |
| 8 | Paint House III (1473) | Neighborhoods constraint |
| 9 | Paint Fence (276) | Same/different counting |

### Other State Machines
| # | Problem | Key Learning |
|---|---------|--------------|
| 10 | Flip String to Monotone Increasing (926) | 0/1 state |
| 11 | Student Attendance Record II (552) | A count + L streak |
| 12 | Maximum Length of Repeated Subarray (718) | State = match length |
| 13 | Dungeon Game (174) | Reverse DP with health state |
| 14 | Cherry Pickup (741) | Two paths simultaneously |

---

## 22. DP — Bitmask (16 problems)

### Basic Subset DP
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Partition to K Equal Sum Subsets (698) | Subset enumeration |
| 2 | Matchsticks to Square (473) | 4 equal subsets |
| 3 | Number of Ways to Wear Different Hats (1434) | Assignment problem |
| 4 | Minimum Number of Work Sessions (1986) | Subset DP |

### Path + Bitmask
| # | Problem | Key Learning |
|---|---------|--------------|
| 5 | Shortest Path Visiting All Nodes (847) | BFS + bitmask |
| 6 | Find Shortest Superstring (943) | TSP variant |
| 7 | Parallel Courses II (1494) | Topo + bitmask |

### Grid + Bitmask (Profile DP)
| # | Problem | Key Learning |
|---|---------|--------------|
| 8 | Maximum Students Taking Exam (1349) | Row bitmask |
| 9 | Minimum Cost to Connect Two Groups (1595) | Two groups bitmask |
| 10 | Number of Ways to Build House (2320) | Profile DP |

### Subset Sum/Count
| # | Problem | Key Learning |
|---|---------|--------------|
| 11 | Can I Win (464) | Game with bitmask |
| 12 | Stickers to Spell Word (691) | Bitmask + memoization |
| 13 | Beautiful Arrangement (526) | Permutation counting |

### Advanced Bitmask
| # | Problem | Key Learning |
|---|---------|--------------|
| 14 | Maximum AND Sum of Array (2172) | Assignment to slots |
| 15 | Smallest Sufficient Team (1125) | Minimum subset cover |
| 16 | Distribute Repeating Integers (1655) | Subset assignment |

---

## 23. DP — Digit DP (8 problems)

| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Numbers At Most N Given Digit Set (902) | Basic digit DP |
| 2 | Count of Integers (2719) | Digit DP template |
| 3 | Numbers With Repeated Digits (1012) | Count without repeats |
| 4 | Non-negative Integers without Consecutive Ones (600) | Fibonacci connection |
| 5 | Count Special Integers (2376) | Distinct digits |
| 6 | Number of Digit One (233) | Count specific digit |
| 7 | Count Numbers with Unique Digits (357) | Permutation counting |
| 8 | Digit Count in Range (1067) | Range digit frequency |

---

## 24. Greedy (18 problems)

### Interval Scheduling
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Non-overlapping Intervals (435) | Maximum intervals |
| 2 | Minimum Number of Arrows (452) | Merge overlapping |
| 3 | Meeting Rooms II (253) | Minimum rooms |
| 4 | Insert Interval (57) | Insert and merge |
| 5 | Merge Intervals (56) | Standard merge |

### Array Greedy
| # | Problem | Key Learning |
|---|---------|--------------|
| 6 | Jump Game (55) | Can reach end |
| 7 | Jump Game II (45) | Minimum jumps (BFS-like) |
| 8 | Candy (135) | Two pass greedy |
| 9 | Gas Station (134) | Circular greedy |
| 10 | Patching Array (330) | Non-obvious greedy |

### Two Heaps / Scheduling
| # | Problem | Key Learning |
|---|---------|--------------|
| 11 | Task Scheduler (621) | Frequency-based greedy |
| 12 | IPO (502) | Two heaps |
| 13 | Course Schedule III (630) | Greedy + heap |
| 14 | Single-Threaded CPU (1834) | Sort + heap |

### String Greedy
| # | Problem | Key Learning |
|---|---------|--------------|
| 15 | Reorganize String (767) | Greedy placement |
| 16 | Smallest Subsequence of Distinct Characters (1081) | Monotonic + greedy |

### Advanced Greedy
| # | Problem | Key Learning |
|---|---------|--------------|
| 17 | Minimum Number of Refueling Stops (871) | Heap greedy |
| 18 | Maximum Performance of a Team (1383) | Sort + heap |

---

## DP — Additional Missing Topics

### DP with Monotonic Queue Optimization
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Constrained Subsequence Sum (1425) | Deque for sliding max |
| 2 | Jump Game VI (1696) | Same pattern |
| 3 | Max Value of Equation (1499) | Deque optimization |
| 4 | Shortest Subarray with Sum at Least K (862) | Prefix + deque |
| 5 | Maximum Number of Books You Can Take (2355) | Stack + DP |

### Probability / Expected Value DP
| # | Problem | Key Learning |
|---|---------|--------------|
| 6 | Knight Probability in Chessboard (688) | Grid probability |
| 7 | Soup Servings (808) | Memoization with pruning |
| 8 | New 21 Game (837) | Sliding window probability |
| 9 | Toss Strange Coins (1230) | Coin flip probability |
| 10 | Probability of a Two Boxes Having Same Number of Balls (1467) | Complex counting |

### Game Theory DP
| # | Problem | Key Learning |
|---|---------|--------------|
| 11 | Stone Game (877) | Optimal play |
| 12 | Stone Game II (1140) | Variable take |
| 13 | Stone Game IV (1510) | Square number game |
| 14 | Predict the Winner (486) | Same as Stone Game |
| 15 | Can I Win (464) | Bitmask + game |
| 16 | Flip Game II (294) | Memoized game |

### Matrix Exponentiation DP
| # | Problem | Key Learning |
|---|---------|--------------|
| 17 | Knight Dialer (935) | State transitions as matrix |
| 18 | Domino and Tromino Tiling (790) | Recurrence to matrix |
| 19 | Number of Ways to Stay in the Same Place (1269) | Position + steps |
| 20 | Count Vowels Permutation (1220) | Character transition matrix |
| 21 | Student Attendance Record II (552) | Already have, matrix speedup possible |

### SOS DP (Sum over Subsets)
| # | Problem | Key Learning |
|---|---------|--------------|
| 22 | Count Number of Maximum Bitwise-OR Subsets (2044) | Basic SOS |
| 23 | Closest Subsequence Sum (1755) | Meet in middle + SOS |
| 24 | Number of Wonderful Substrings (1915) | Bitmask + counting |
| 25 | Find XOR Sum of All Pairs Bitwise AND (1835) | Bit manipulation |

### DP on Trees (Additional)
| # | Problem | Key Learning |
|---|---------|--------------|
| 26 | Longest ZigZag Path in Binary Tree (1372) | Direction state |
| 27 | Maximum Sum BST in Binary Tree (1373) | Validate + compute |
| 28 | Number of Ways to Reorder Array to Get Same BST (1569) | Combinatorics + tree |
| 29 | Create Components With Same Value (2440) | Factor enumeration + tree DP |
| 30 | Collect Coins in a Tree (2603) | Topological peel + DP |

### Advanced Interval DP
| # | Problem | Key Learning |
|---|---------|--------------|
| 31 | Minimum Cost to Cut a Stick (1547) | Classic interval |
| 32 | Stone Game VII (1690) | Remove-based interval |
| 33 | Maximize Score After N Operations (1799) | Bitmask meets interval |
| 34 | Minimum Cost to Merge Stones (1000) | Already have, but essential |

### Advanced Linear DP
| # | Problem | Key Learning |
|---|---------|--------------|
| 35 | Count Different Palindromic Subsequences (730) | 4 chars, complex counting |
| 36 | Minimum Difficulty of a Job Schedule (1335) | Partition DP |
| 37 | Maximum Number of Points with Cost (1937) | Optimize O(n²) to O(n) |
| 38 | Minimum White Tiles After Covering With Carpets (2209) | Cover DP |
| 39 | Number of Ways to Divide a Long Corridor (2147) | Counting with constraints |
| 40 | Number of People Aware of a Secret (2327) | Range-based spreading |

### Profile DP / Broken Profile
| # | Problem | Key Learning |
|---|---------|--------------|
| 41 | Domino and Tromino Tiling (790) | Simple profile |
| 42 | Number of Ways to Build House of Cards (2189) | Profile DP |

---

## 25. Heap / Priority Queue (14 problems)

### Top K / Kth Element
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Kth Largest Element in Array (215) | Quickselect or heap |
| 2 | Top K Frequent Elements (347) | Heap or bucket sort |
| 3 | Top K Frequent Words (692) | Custom comparator |
| 4 | K Closest Points to Origin (973) | Max heap of size k |

### Two Heaps
| # | Problem | Key Learning |
|---|---------|--------------|
| 5 | Find Median from Data Stream (295) | Classic two heaps |
| 6 | Sliding Window Median (480) | Two heaps + lazy deletion |
| 7 | IPO (502) | Two heaps for selection |

### Merge Streams
| # | Problem | Key Learning |
|---|---------|--------------|
| 8 | Merge k Sorted Lists (23) | K-way merge |
| 9 | Smallest Range Covering Elements (632) | K-way with window |
| 10 | Find K Pairs with Smallest Sums (373) | BFS-like with heap |

### Advanced Heap
| # | Problem | Key Learning |
|---|---------|--------------|
| 11 | Trapping Rain Water II (407) | 2D BFS + min heap |
| 12 | Swim in Rising Water (778) | Dijkstra-like |
| 13 | The Skyline Problem (218) | Sweep line + heap |
| 14 | Maximum Frequency Stack (895) | Heap or stack of stacks |

---

## Heap — Additional Variations

### Lazy Deletion Heap
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Sliding Window Median (480) | Two heaps + lazy deletion |
| 2 | The Skyline Problem (218) | Heap + lazy removal |
| 3 | Design a Number Container System (2349) | Track validity |

### Simulation with Heap
| # | Problem | Key Learning |
|---|---------|--------------|
| 4 | Meeting Rooms III (2402) | Room assignment simulation |
| 5 | Process Tasks Using Servers (1882) | Available + busy heaps |
| 6 | Single-Threaded CPU (1834) | Sort + heap simulation |
| 7 | Seat Reservation Manager (1845) | Min available seat |

### Greedy + Heap
| # | Problem | Key Learning |
|---|---------|--------------|
| 8 | Minimum Cost to Hire K Workers (857) | Ratio sorting + heap |
| 9 | Maximum Subsequence Score (2542) | Sort + maintain k elements |
| 10 | Maximum Performance of a Team (1383) | Sort by one, heap other |
| 11 | Furthest Building You Can Reach (1642) | Greedy resource allocation |
| 12 | Longest Happy String (1405) | Greedy character placement |

### Heap for Optimization
| # | Problem | Key Learning |
|---|---------|--------------|
| 13 | Minimize Deviation in Array (1675) | Normalize then min heap |
| 14 | Minimum Operations to Halve Array Sum (2208) | Always halve maximum |
| 15 | Remove Stones to Minimize the Total (1962) | Similar pattern |
| 16 | Maximum Average Pass Ratio (1792) | Marginal gain heap |
| 17 | Maximal Score After Applying K Operations (2530) | Ceil division |

### Multi-Heap Patterns
| # | Problem | Key Learning |
|---|---------|--------------|
| 18 | Total Cost to Hire K Workers (2462) | Two heaps from ends |
| 19 | Find Score of an Array After Marking All Elements (2593) | Heap with marking |
| 20 | IPO (502) | Unlock projects as capital grows |

---

## 26. Trie (10 problems)

### Basic Trie Operations
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Implement Trie (208) | Basic implementation |
| 2 | Design Add and Search Words (211) | Wildcard search |
| 3 | Replace Words (648) | Prefix replacement |
| 4 | Map Sum Pairs (677) | Trie with values |

### Trie + Backtracking
| # | Problem | Key Learning |
|---|---------|--------------|
| 5 | Word Search II (212) | Board search with trie |
| 6 | Concatenated Words (472) | Word composition |

### Bitwise Trie
| # | Problem | Key Learning |
|---|---------|--------------|
| 7 | Maximum XOR of Two Numbers (421) | XOR trie |
| 8 | Maximum XOR With Element From Array (1707) | Offline + sorted queries |

### Advanced Trie
| # | Problem | Key Learning |
|---|---------|--------------|
| 9 | Palindrome Pairs (336) | Reverse lookup |
| 10 | Design Search Autocomplete (642) | Trie + ranking |

---

## 27. Segment Tree / BIT (14 problems)

### Basic Range Queries
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Range Sum Query - Mutable (307) | Basic segment tree or BIT |
| 2 | Range Sum Query 2D - Mutable (308) | 2D BIT |

### Inversion Counting
| # | Problem | Key Learning |
|---|---------|--------------|
| 3 | Count of Smaller Numbers After Self (315) | BIT or merge sort |
| 4 | Reverse Pairs (493) | Modified merge sort or BIT |
| 5 | Count of Range Sum (327) | Merge sort or BIT |
| 6 | Create Sorted Array Through Instructions (1649) | BIT for inversions |

### Coordinate Compression
| # | Problem | Key Learning |
|---|---------|--------------|
| 7 | Falling Squares (699) | Segment tree + compression |
| 8 | My Calendar I, II, III (729, 731, 732) | Segment tree or sweep |
| 9 | Rectangle Area II (850) | Sweep line + segment tree |

### Lazy Propagation
| # | Problem | Key Learning |
|---|---------|--------------|
| 10 | Range Module (715) | Segment tree with lazy |
| 11 | Amount of New Area Painted Each Day (2158) | Interval painting |

### Advanced
| # | Problem | Key Learning |
|---|---------|--------------|
| 12 | Longest Increasing Subsequence II (2407) | Segment tree for range max |
| 13 | Count Good Triplets in an Array (2179) | Two BITs |
| 14 | Stamping the Grid (2132) | 2D prefix + segment tree |

---

## 28. String Algorithms (12 problems)

### KMP / Pattern Matching
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Implement strStr (28) | KMP template |
| 2 | Repeated Substring Pattern (459) | KMP failure function |
| 3 | Shortest Palindrome (214) | KMP for palindrome |

### Z-Function
| # | Problem | Key Learning |
|---|---------|--------------|
| 4 | Z-Algorithm Template | Know the technique |
| 5 | Sum of Scores of Built Strings (2223) | Z-function application |

### Rolling Hash (Rabin-Karp)
| # | Problem | Key Learning |
|---|---------|--------------|
| 6 | Longest Duplicate Substring (1044) | Binary search + rolling hash |
| 7 | Distinct Echo Substrings (1316) | Rolling hash counting |
| 8 | Longest Happy Prefix (1392) | KMP or rolling hash |

### Manacher's Algorithm
| # | Problem | Key Learning |
|---|---------|--------------|
| 9 | Longest Palindromic Substring (5) | Manacher's O(n) |
| 10 | Palindromic Substrings (647) | Manacher's application |

### Suffix Array / Advanced
| # | Problem | Key Learning |
|---|---------|--------------|
| 11 | Last Substring in Lexicographical Order (1163) | Suffix array or two pointers |
| 12 | Number of Distinct Substrings (1698) | Suffix array + LCP |

---

## 29. Bit Manipulation (10 problems)

### Basic Techniques
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Single Number (136) | XOR property |
| 2 | Single Number II (137) | Bit counting / state machine |
| 3 | Single Number III (260) | XOR + grouping |
| 4 | Counting Bits (338) | DP with bits |

### Bit Construction
| # | Problem | Key Learning |
|---|---------|--------------|
| 5 | Maximum XOR of Two Numbers (421) | Greedy bit by bit |
| 6 | Maximum AND Sum of Array (2172) | Bitmask DP |
| 7 | Bitwise AND of Numbers Range (201) | Common prefix |

### Subset Enumeration
| # | Problem | Key Learning |
|---|---------|--------------|
| 8 | Subsets (78) | Bit enumeration |
| 9 | Sum of All Subset XOR Totals (1863) | Contribution technique |

### Advanced
| # | Problem | Key Learning |
|---|---------|--------------|
| 10 | Total Hamming Distance (477) | Bit position counting |

---

## 30. Math & Geometry (12 problems)

### Math
| # | Problem | Key Learning |
|---|---------|--------------|
| 1 | Pow(x, n) (50) | Binary exponentiation |
| 2 | Count Primes (204) | Sieve of Eratosthenes |
| 3 | Ugly Number II (264) | Multi-pointer generation |
| 4 | Super Ugly Number (313) | Heap or multi-pointer |
| 5 | Factorial Trailing Zeroes (172) | Count factors of 5 |
| 6 | Perfect Rectangle (391) | Corner counting + area |

### Geometry
| # | Problem | Key Learning |
|---|---------|--------------|
| 7 | Max Points on a Line (149) | GCD for slope |
| 8 | Erect the Fence (587) | Convex hull |
| 9 | Valid Square (593) | Distance checking |
| 10 | Rectangle Area II (850) | Sweep line |

### Number Theory
| # | Problem | Key Learning |
|---|---------|--------------|
| 11 | Greatest Common Divisor of Strings (1071) | GCD application |
| 12 | X of a Kind in a Deck of Cards (914) | GCD of frequencies |

---

## Summary

| Topic | Problem Count |
|-------|---------------|
| Sliding Window | 18 |
| Two Pointers | 14 |
| Monotonic Stack | 16 |
| Binary Search | 20 |
| Linked List | 15 |
| Trees - Traversal & Construction | 18 |
| Trees - BST | 10 |
| Trees - LCA | 8 |
| Trees - DP | 12 |
| Graphs - BFS | 16 |
| Graphs - DFS | 14 |
| Graphs - Topological Sort | 10 |
| Graphs - Shortest Path | 12 |
| Graphs - Union Find | 12 |
| Graphs - Advanced | 10 |
| Backtracking | 16 |
| DP - Linear | 18 |
| DP - Knapsack | 15 |
| DP - Two Sequences | 12 |
| DP - Interval | 12 |
| DP - State Machine | 14 |
| DP - Bitmask | 16 |
| DP - Digit DP | 8 |
| Greedy | 18 |
| Heap | 14 |
| Trie | 10 |
| Segment Tree / BIT | 14 |
| String Algorithms | 12 |
| Bit Manipulation | 10 |
| Math & Geometry | 12 |
| **TOTAL** | **~400** |

---

## Summary of Additions

| Topic | New Problems |
|-------|--------------|
| Sliding Window | +18 |
| Monotonic Stack/Deque | +21 |
| Binary Search | +23 |
| Union Find | +24 |
| Graphs (various) | +21 |
| DP (various) | +40 |
| Heap | +20 |
| **Total New** | **~167** |

Combined with original ~400, you now have **~567 problems** covering every variation that appears in interviews.



# If you get time or Curious

## Hybrid Problems: Multi-Topic Combinations

These are the problems that separate good candidates from great ones. Each requires recognizing and combining 2-3 techniques.

---

## Binary Search + Greedy

| # | Problem | Techniques | Key Insight |
|---|---------|------------|-------------|
| 1 | Split Array Largest Sum (410) | BS on answer + greedy partition | Check if can split with max sum ≤ mid |
| 2 | Capacity To Ship Packages (1011) | BS on answer + greedy assign | Same pattern |
| 3 | Minimum Time to Complete Trips (2187) | BS on answer + math feasibility | Sum of trips at time t |
| 4 | Maximum Number of Tasks You Can Assign (2071) | BS on answer + greedy + deque | Complex feasibility check |
| 5 | Minimized Maximum of Products Distributed (2064) | BS on answer + greedy distribute | Ceiling division count |
| 6 | Magnetic Force Between Two Balls (1552) | BS on answer + greedy placement | Maximize minimum distance |
| 7 | Maximum Candies You Can Get from Boxes (1298) | BS + simulation | Multi-state feasibility |
| 8 | Koko Eating Bananas (875) | BS on answer + greedy | Foundation problem |

---

## Binary Search + DP

| # | Problem | Techniques | Key Insight |
|---|---------|------------|-------------|
| 1 | Longest Increasing Subsequence (300) | DP + BS for O(n log n) | Patience sorting |
| 2 | Russian Doll Envelopes (354) | Sort + LIS with BS | 2D to 1D reduction |
| 3 | Maximum Profit in Job Scheduling (1235) | DP + BS for previous job | Binary search on end times |
| 4 | Longest Common Subsequence (1143) + Hunt-Szymanski | BS optimization on matches | For specific cases |
| 5 | Closest Subsequence Sum (1755) | Meet in middle + BS | Split array, search sums |
| 6 | Super Egg Drop (887) | DP + BS on drop floor | Optimize transition |
| 7 | Tallest Billboard (956) | DP + state optimization | Difference as state |
| 8 | Number of Longest Increasing Subsequence (673) | DP + BS + segment tree | Count LIS |

---

## Binary Search + Graph (BFS/DFS)

| # | Problem | Techniques | Key Insight |
|---|---------|------------|-------------|
| 1 | Swim in Rising Water (778) | BS on answer + BFS/DFS check | Can reach with max ≤ mid? |
| 2 | Path With Minimum Effort (1631) | BS + BFS or Dijkstra | Minimize max edge |
| 3 | Escape the Spreading Fire (2258) | BS on wait time + multi-source BFS | Fire BFS + person BFS |
| 4 | Minimum Time to Visit a Cell (2577) | BS concept + Dijkstra with parity | Time + parity state |
| 5 | Minimum Number of Days to Disconnect Island (1568) | BS concept + articulation points | 0, 1, or 2 days |
| 6 | Kth Smallest Instructions (1643) | BS concept + combinatorics | Lexicographic path |
| 7 | Minimize the Maximum Edge Weight (2699) | BS + BFS/MST | Edge weight threshold |

---

## Sliding Window + Monotonic Deque

| # | Problem | Techniques | Key Insight |
|---|---------|------------|-------------|
| 1 | Sliding Window Maximum (239) | Fixed window + max deque | Classic combination |
| 2 | Shortest Subarray with Sum at Least K (862) | Prefix + monotonic deque | Handles negatives |
| 3 | Longest Continuous Subarray With Absolute Diff ≤ Limit (1438) | Variable window + min/max deques | Two deques |
| 4 | Constrained Subsequence Sum (1425) | DP + monotonic deque | Optimize DP transition |
| 5 | Jump Game VI (1696) | DP + sliding window max | Same as above |
| 6 | Max Value of Equation (1499) | Deque maintaining y-x | Transform equation |
| 7 | Maximum Number of Robots Within Budget (2398) | Window + deque + sum | Multi-constraint window |
| 8 | Maximum Sum of 3 Non-Overlapping Subarrays (689) | Prefix + DP + sliding idea | Track best left/right |

---

## Prefix Sum + Monotonic Stack

| # | Problem | Techniques | Key Insight |
|---|---------|------------|-------------|
| 1 | Sum of Subarray Minimums (907) | Stack + contribution counting | Each element's range |
| 2 | Sum of Subarray Ranges (2104) | Stack for min + stack for max | Difference of contributions |
| 3 | Sum of Total Strength of Wizards (2281) | Stack + prefix of prefix | Very hard combination |
| 4 | Maximum Score of a Good Subarray (1793) | Stack or two pointers | Expand from index k |
| 5 | Largest Rectangle in Histogram (84) | Stack for boundaries | Width × height |
| 6 | Maximal Rectangle (85) | Histogram per row | Build on 84 |
| 7 | Trapping Rain Water (42) | Stack or prefix max | Multiple approaches |

---

## Tree DP + DFS

| # | Problem | Techniques | Key Insight |
|---|---------|------------|-------------|
| 1 | Binary Tree Maximum Path Sum (124) | DFS + track global vs return | Classic split |
| 2 | Binary Tree Cameras (968) | Post-order + 3 states | Greedy on tree |
| 3 | Sum of Distances in Tree (834) | Two DFS + rerooting | Change root technique |
| 4 | Difference Between Maximum and Minimum Price Sum (2538) | Rerooting DP | Same technique |
| 5 | Distribute Coins in Binary Tree (979) | DFS + flow counting | Excess/deficit |
| 6 | House Robber III (337) | DFS + rob/skip state | State DP on tree |
| 7 | Longest Path With Different Adjacent Characters (2246) | DFS + track two longest | Extension of diameter |
| 8 | Maximum Product of Splitted Binary Tree (1339) | Two DFS: total sum, then check splits | Prefix knowledge |
| 9 | Count Number of Possible Root Nodes (2581) | Rerooting + counting | Guess validation |
| 10 | Collect Coins in a Tree (2603) | Topological peel + distance | Remove leaves iteratively |

---

## Graph + DP

| # | Problem | Techniques | Key Insight |
|---|---------|------------|-------------|
| 1 | Longest Increasing Path in Matrix (329) | DFS + memoization | Topological nature |
| 2 | Cheapest Flights Within K Stops (787) | BFS/Bellman-Ford + state | (node, stops) state |
| 3 | Parallel Courses III (2050) | Topological sort + DP | Time = max dependency + self |
| 4 | Number of Ways to Arrive at Destination (1976) | Dijkstra + count paths | Count at same distance |
| 5 | Shortest Path Visiting All Nodes (847) | BFS + bitmask | State = (node, visited mask) |
| 6 | Find Shortest Superstring (943) | Graph + bitmask DP (TSP) | Overlap as edge weight |
| 7 | Minimum Cost to Reach Destination in Time (1928) | Dijkstra + time constraint | (node, time) state |
| 8 | Frog Jump (403) | DFS/BFS + (position, jump) state | State space search |
| 9 | Cat and Mouse (913) | BFS from terminal + game state | (mouse, cat, turn) |
| 10 | Minimum Weighted Subgraph With Required Paths (2203) | 3 Dijkstras + meet in middle | src1, src2, reverse from dest |

---

## Graph + Union Find

| # | Problem | Techniques | Key Insight |
|---|---------|------------|-------------|
| 1 | Accounts Merge (721) | Union Find + DFS/BFS for result | Group then collect |
| 2 | Redundant Connection II (685) | Union Find + directed edge cases | Two candidates scenario |
| 3 | Checking Existence of Edge Length Limited Paths (1697) | Offline + sort + Union Find | Process queries by weight |
| 4 | Number of Good Paths (2421) | Union Find + sorted values | Connect as values increase |
| 5 | Bricks Falling When Hit (803) | Reverse Union Find | Time reversal technique |
| 6 | Making A Large Island (827) | Union Find + try each 0 | Component labeling |
| 7 | Remove Max Number of Edges (1579) | Two Union Finds | Alice and Bob separately |
| 8 | Minimize Malware Spread II (928) | Union Find + analysis | Try removing each infected |

---

## Heap + Greedy

| # | Problem | Techniques | Key Insight |
|---|---------|------------|-------------|
| 1 | IPO (502) | Two heaps + unlock mechanism | Capital threshold |
| 2 | Course Schedule III (630) | Sort + max heap for replacement | Swap if better |
| 3 | Minimum Cost to Hire K Workers (857) | Sort by ratio + heap for sum | Ratio determines pay |
| 4 | Maximum Performance of a Team (1383) | Sort by efficiency + heap | Fix minimum, optimize sum |
| 5 | Maximum Subsequence Score (2542) | Same pattern as above | Sort + maintain k |
| 6 | Task Scheduler (621) | Greedy frequency OR heap | Cooldown handling |
| 7 | Reorganize String (767) | Heap for most frequent | Interleave characters |
| 8 | Meeting Rooms III (2402) | Sort + two heaps | Available + busy rooms |
| 9 | Single-Threaded CPU (1834) | Sort by arrival + min heap | Process simulation |
| 10 | Minimum Number of Refueling Stops (871) | Greedy + max heap | Retrospective refuel |

---

## Heap + Graph (Dijkstra Variants)

| # | Problem | Techniques | Key Insight |
|---|---------|------------|-------------|
| 1 | Network Delay Time (743) | Standard Dijkstra | Foundation |
| 2 | Path With Maximum Probability (1514) | Max-heap Dijkstra | Flip to max |
| 3 | Swim in Rising Water (778) | Dijkstra on max edge | Minimize maximum |
| 4 | Path With Minimum Effort (1631) | Same as above | Same pattern |
| 5 | Trapping Rain Water II (407) | Multi-source Dijkstra from border | 2D water filling |
| 6 | The Maze II (505) | Dijkstra with rolling | Stop at wall |
| 7 | Reachable Nodes In Subdivided Graph (882) | Dijkstra + fractional counting | Count reachable nodes |
| 8 | Second Minimum Time to Reach Destination (2045) | Track two best per node | Second shortest path |

---

## Trie + Backtracking/DFS

| # | Problem | Techniques | Key Insight |
|---|---------|------------|-------------|
| 1 | Word Search II (212) | Trie + grid DFS | Prune with trie |
| 2 | Palindrome Pairs (336) | Trie + reverse lookup | Check prefix/suffix |
| 3 | Concatenated Words (472) | Trie + DFS word break | Can form from others |
| 4 | Stream of Characters (1032) | Reverse trie + rolling | Match suffixes |
| 5 | Design Search Autocomplete System (642) | Trie + ranking | Hot sentences |
| 6 | Maximum XOR of Two Numbers (421) | Bitwise trie + greedy | Maximize bit by bit |
| 7 | Maximum XOR With Element From Array (1707) | Sort queries + trie | Offline processing |

---

## Segment Tree/BIT + DP

| # | Problem | Techniques | Key Insight |
|---|---------|------------|-------------|
| 1 | Count of Smaller Numbers After Self (315) | BIT/merge sort + inversion | Count inversions |
| 2 | Reverse Pairs (493) | Merge sort + counting | Modified inversion |
| 3 | Count of Range Sum (327) | Merge sort OR BIT | Range counting |
| 4 | Longest Increasing Subsequence II (2407) | Segment tree for range max | DP optimization |
| 5 | Create Sorted Array through Instructions (1649) | BIT for cost counting | Inversions on insert |
| 6 | Count Good Triplets in an Array (2179) | Two BITs | Count before and after |
| 7 | Maximum Sum Queries (2736) | Segment tree + offline | Query processing |
| 8 | Booking Concert Tickets in Groups (2286) | Segment tree with lazy | Range operations |

---

## Bitmask + BFS/Graph

| # | Problem | Techniques | Key Insight |
|---|---------|------------|-------------|
| 1 | Shortest Path Visiting All Nodes (847) | BFS + bitmask state | (node, visited) |
| 2 | Shortest Path to Get All Keys (864) | BFS + key bitmask | (position, keys) |
| 3 | Find Shortest Superstring (943) | TSP with bitmask | Overlap graph |
| 4 | Minimum Number of Days to Eat N Oranges (1553) | BFS/memo + math | State = remaining |
| 5 | Parallel Courses II (1494) | Topo + bitmask DP | Which k to take |
| 6 | Smallest Sufficient Team (1125) | Bitmask DP | Minimum cover |
| 7 | Maximum Students Taking Exam (1349) | Row bitmask DP | Profile DP |

---

## Stack + DP

| # | Problem | Techniques | Key Insight |
|---|---------|------------|-------------|
| 1 | Longest Valid Parentheses (32) | Stack OR DP | Track valid lengths |
| 2 | Maximal Rectangle (85) | Stack (histogram) per row | Build row by row |
| 3 | Largest Rectangle in Histogram (84) | Stack for boundaries | Foundation |
| 4 | Maximum Number of Books You Can Take (2355) | Stack + arithmetic DP | Decreasing constraint |
| 5 | Odd Even Jump (975) | Monotonic stack + DP | Can reach end? |
| 6 | 132 Pattern (456) | Stack tracking max on right | Reverse traversal |
| 7 | Sum of Subarray Minimums (907) | Stack + contribution DP | Already covered |

---

## Two Pointers + Binary Search

| # | Problem | Techniques | Key Insight |
|---|---------|------------|-------------|
| 1 | 3Sum Closest (16) | Sort + two pointers + track best | Minimize difference |
| 2 | Find K-th Smallest Pair Distance (719) | BS on answer + two pointer count | Count pairs ≤ mid |
| 3 | Kth Smallest Element in Sorted Matrix (378) | BS + count via diagonal | Count ≤ mid |
| 4 | Kth Smallest Number in Multiplication Table (668) | BS + row-wise count | Same pattern |
| 5 | K-th Smallest Prime Fraction (786) | BS on value + two pointer | Fraction searching |
| 6 | Longest Substring with At Least K Repeating (395) | Enumerate unique + two pointer | Or divide conquer |
| 7 | Subarray Product Less Than K (713) | Two pointers with product | Shrink window |

---

## LCA + Path Queries (Binary Lifting)

| # | Problem | Techniques | Key Insight |
|---|---------|------------|-------------|
| 1 | Kth Ancestor of a Tree Node (1483) | Binary lifting | 2^k jumps |
| 2 | Lowest Common Ancestor of Binary Tree (236) | DFS or binary lifting | Foundation |
| 3 | Maximum Difference Between Node and Ancestor (1026) | DFS + track min/max | Path extremes |
| 4 | Minimum Edge Weight Equilibrium Queries (2846) | LCA + frequency tracking | Path queries |
| 5 | Closest Node to Path in Tree (2277) | LCA + distance | Path distance |
| 6 | Number of Nodes in Sub-Tree With Same Label (1519) | DFS + frequency array | Subtree counting |
| 7 | Distance in a Binary Tree (1740) | LCA + distance formula | dist(a,b) = dist(a,lca) + dist(b,lca) |

---

## Meet in the Middle

| # | Problem | Techniques | Key Insight |
|---|---------|------------|-------------|
| 1 | Closest Subsequence Sum (1755) | Split + enumerate both halves | 2^20 each half |
| 2 | Partition Array Into Two Arrays to Minimize Sum Difference (2035) | Meet in middle + BS | Balance sums |
| 3 | Number of Ways to Reorder Array to Get Same BST (1569) | Combinatorics + divide | Left/right independence |
| 4 | 4Sum II (454) | Two pairs hashing | A+B vs -(C+D) |
| 5 | Split Array With Same Average (805) | Subset sum + meet in middle | Complex feasibility |

---

## Sweep Line + Data Structure

| # | Problem | Techniques | Key Insight |
|---|---------|------------|-------------|
| 1 | The Skyline Problem (218) | Sweep + heap/multiset | Track active heights |
| 2 | Meeting Rooms II (253) | Sweep or heap | Count overlaps |
| 3 | My Calendar III (732) | Sweep line or segment tree | Max concurrent |
| 4 | Rectangle Area II (850) | Sweep + segment tree | Area computation |
| 5 | Falling Squares (699) | Sweep + segment tree | Track heights |
| 6 | Amount of New Area Painted Each Day (2158) | Sweep + interval tracking | Paint intervals |
| 7 | Describe the Painting (1943) | Sweep line + color mixing | Segment changes |

---

## Frequently Asked in Interviews (Top 50 Hybrids)

These appear most often based on interview frequency:

| Rank | Problem | Companies | Combination |
|------|---------|-----------|-------------|
| 1 | LRU Cache (146) | All FAANG | Hashmap + Doubly Linked List |
| 2 | Merge k Sorted Lists (23) | All FAANG | Heap + Linked List |
| 3 | Word Search II (212) | Google, Meta | Trie + Backtracking |
| 4 | Trapping Rain Water (42) | All FAANG | Stack/Two Pointer + Prefix |
| 5 | Median from Data Stream (295) | Amazon, Google | Two Heaps |
| 6 | Maximum Profit Job Scheduling (1235) | Google, Airbnb | DP + Binary Search |
| 7 | Alien Dictionary (269) | Meta, Google | Graph + Topological Sort |
| 8 | Sliding Window Maximum (239) | Amazon, Google | Window + Monotonic Deque |
| 9 | Serialize/Deserialize Binary Tree (297) | All FAANG | Tree + BFS/DFS |
| 10 | Binary Tree Maximum Path Sum (124) | Meta, Google | Tree DP |
| 11 | Accounts Merge (721) | Meta | Union Find + DFS |
| 12 | Word Ladder (127) | Amazon, Meta | BFS + String |
| 13 | Longest Increasing Subsequence (300) | All | DP + Binary Search |
| 14 | Course Schedule II (210) | All | Graph + Topological Sort |
| 15 | The Skyline Problem (218) | Google, Microsoft | Sweep + Heap |
| 16 | Minimum Window Substring (76) | Meta, Amazon | Sliding Window + Hashmap |
| 17 | Largest Rectangle Histogram (84) | Google, Amazon | Monotonic Stack |
| 18 | Edit Distance (72) | Google, Amazon | Two Sequence DP |
| 19 | Regular Expression Matching (10) | Google, Meta | DP + String |
| 20 | Shortest Path Visiting All Nodes (847) | Google | BFS + Bitmask |
| 21 | Find Median in Two Sorted Arrays (4) | Google, Amazon | Binary Search |
| 22 | Critical Connections (1192) | Amazon | Tarjan's Algorithm |
| 23 | Number of Islands II (305) | Google, Meta | Union Find + Grid |
| 24 | Task Scheduler (621) | Meta, Amazon | Greedy + Heap/Math |
| 25 | LFU Cache (460) | Amazon, Google | Hashmap + Doubly Linked List |
| 26 | Split Array Largest Sum (410) | Google | BS + Greedy |
| 27 | Burst Balloons (312) | Google | Interval DP |
| 28 | Swim in Rising Water (778) | Google | BS + BFS / Dijkstra |
| 29 | Cheapest Flights K Stops (787) | Airbnb, Amazon | Graph + DP |
| 30 | Count of Smaller After Self (315) | Google, Amazon | BIT / Merge Sort |
| 31 | Maximal Rectangle (85) | Google, Meta | Stack + DP |
| 32 | Subarrays with K Different Integers (992) | Uber, Google | Sliding Window |
| 33 | Maximum XOR of Two Numbers (421) | Google | Bitwise Trie |
| 34 | Minimum Cost to Hire K Workers (857) | Google | Sort + Heap |
| 35 | Number of Good Paths (2421) | Google | Union Find + Sort |
| 36 | Best Time Buy Stock IV (188) | Amazon | State Machine DP |
| 37 | Palindrome Pairs (336) | Airbnb, Google | Trie + String |
| 38 | Range Sum Query 2D Mutable (308) | Google | 2D BIT |
| 39 | Russian Doll Envelopes (354) | Google | Sort + LIS |
| 40 | Meeting Rooms III (2402) | Google | Heap + Simulation |
| 41 | Sum of Subarray Minimums (907) | Amazon | Stack + Contribution |
| 42 | Minimum Interval to Include Query (1851) | Google | Sort + Heap |
| 43 | Maximum Frequency Stack (895) | Amazon | Stack + Hashmap |
| 44 | Design Search Autocomplete (642) | Google, Amazon | Trie + Heap |
| 45 | Shortest Subarray Sum ≥ K (862) | Google | Prefix + Deque |
| 46 | Longest Valid Parentheses (32) | Amazon | Stack + DP |
| 47 | IPO (502) | Amazon | Two Heaps |
| 48 | Trapping Rain Water II (407) | Google | Heap + BFS |
| 49 | Making A Large Island (827) | Meta, Google | Union Find + Grid |
| 50 | Closest Subsequence Sum (1755) | Google | Meet in Middle |

---

## Summary

| Category | Problem Count |
|----------|---------------|
| Binary Search + Greedy | 8 |
| Binary Search + DP | 8 |
| Binary Search + Graph | 7 |
| Sliding Window + Monotonic Deque | 8 |
| Prefix Sum + Monotonic Stack | 7 |
| Tree DP + DFS | 10 |
| Graph + DP | 10 |
| Graph + Union Find | 8 |
| Heap + Greedy | 10 |
| Heap + Graph | 8 |
| Trie + Backtracking | 7 |
| Segment Tree + DP | 8 |
| Bitmask + BFS/Graph | 7 |
| Stack + DP | 7 |
| Two Pointers + Binary Search | 7 |
| LCA + Path Queries | 7 |
| Meet in the Middle | 5 |
| Sweep Line + DS | 7 |
| **Top 50 Interview Hybrids** | 50 |
| **Total New** | **~140 unique** |

---
