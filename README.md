# Top 50 DSA Problems for Senior C++ Interviews

This list is compiled based on frequently asked problems in senior-level interviews at companies like Amazon, Google, and Microsoft, drawn from popular sources such as Blind 75, LeetCode Top Interview 150, and other curated DSA sheets. Problems are sorted by topic, focusing on medium to hard difficulties for senior roles. Each entry includes the problem name, LeetCode ID (LC#), difficulty, a brief description, and why it's frequently asked (e.g., tests specific patterns like two pointers or DP states).

I've selected ~5 problems per main topic to reach approximately 50, prioritizing frequency from FAANG trends. For C++-specific interviews, emphasize efficient implementations (e.g., using std::unordered_map for hashing, std::priority_queue for heaps).

## 1. Arrays & Strings
These test two pointers, sliding windows, prefix sums, and string manipulations.

1. **Two Sum (LC1, Easy)**  
   Description: Given an array of integers and a target, return indices of two numbers that add up to the target.  
   Why frequent: Tests hashing for O(1) lookups; common warmup for sum variations in Amazon/Google interviews.

2. **3Sum (LC15, Medium)**  
   Description: Find all unique triplets in an array that sum to zero.  
   Why frequent: Builds on two-sum with sorting and two pointers; often in Microsoft for multi-sum problems.

3. **Container With Most Water (LC11, Medium)**  
   Description: Given heights of lines, find two lines that form a container with max area.  
   Why frequent: Classic two-pointer optimization; tests greedy choices in Amazon.

4. **Longest Substring Without Repeating Characters (LC3, Medium)**  
   Description: Find the length of the longest substring without repeating characters.  
   Why frequent: Sliding window with hash set; common in Google for string window problems.

5. **Group Anagrams (LC49, Medium)**  
   Description: Group a list of strings by their anagrams.  
   Why frequent: Hashing with sorted keys; tests map usage in C++ for frequency/counting.

## 2. Linked Lists
Focus on reversals, cycles, and merging; senior interviews may ask for in-place modifications.

6. **Reverse Linked List (LC206, Easy)**  
   Description: Reverse a singly linked list.  
   Why frequent: Basic pointer manipulation; often extended to reverse in groups for Google.

7. **Linked List Cycle (LC141, Easy)**  
   Description: Detect if a cycle exists in a linked list.  
   Why frequent: Floyd's tortoise-hare algorithm; tests cycle detection in Microsoft.

8. **Merge Two Sorted Lists (LC21, Easy)**  
   Description: Merge two sorted linked lists into one.  
   Why frequent: Recursive or iterative merging; common building block for k-merge.

9. **Remove Nth Node From End of List (LC19, Medium)**  
   Description: Remove the nth node from the end of a linked list.  
   Why frequent: Two-pass or one-pass with dummies; tests edge cases in Amazon.

10. **Reorder List (LC143, Medium)**  
    Description: Reorder a list to L0 → Ln → L1 → Ln-1 → ...  
    Why frequent: Combines reverse and merge; senior-level for complex manipulations.

## 3. Stacks & Queues
Emphasize monotonic stacks, deques for windows, and expression handling.

11. **Valid Parentheses (LC20, Easy)**  
    Description: Check if a string of parentheses is valid.  
    Why frequent: Basic stack usage; often in Google as a starter.

12. **Next Greater Element I (LC496, Easy)**  
    Description: Find the next greater element for each in an array.  
    Why frequent: Monotonic stack; extends to daily temperatures in Amazon.

13. **Sliding Window Maximum (LC239, Hard)**  
    Description: Find max in each k-sized window of an array.  
    Why frequent: Deque for O(n) efficiency; common in Microsoft for optimizations.

14. **Evaluate Reverse Polish Notation (LC150, Medium)**  
    Description: Evaluate a postfix expression.  
    Why frequent: Stack for operators; tests infix/postfix conversions.

15. **Implement Queue using Stacks (LC232, Easy)**  
    Description: Implement a queue using two stacks.  
    Why frequent: Understand stack/queue differences; design question variant.

## 4. Hashing / Maps / Sets
Test frequency counting, subarray sums, and cache designs.

16. **Contains Duplicate (LC217, Easy)**  
    Description: Check if an array has duplicates.  
    Why frequent: Simple set usage; warmup for unique elements.

17. **Subarray Sum Equals K (LC560, Medium)**  
    Description: Find number of subarrays summing to k.  
    Why frequent: Prefix sum + hashmap; common in Google for cumulative tricks.

18. **Longest Consecutive Sequence (LC128, Medium)**  
    Description: Find longest sequence of consecutive numbers in unsorted array.  
    Why frequent: Set for O(n) lookup; tests boundary checks in Amazon.

19. **Top K Frequent Elements (LC347, Medium)**  
    Description: Find top k frequent elements in an array.  
    Why frequent: Map + priority queue combo; senior for multi-data structure.

20. **LRU Cache (LC146, Medium)**  
    Description: Design an LRU cache with get/put in O(1).  
    Why frequent: List + map; system design in C++ for Microsoft seniors.

## 5. Trees & Binary Search Trees
Cover traversals, validation, and path sums.

21. **Invert Binary Tree (LC226, Easy)**  
    Description: Flip a binary tree.  
    Why frequent: Recursive traversal; simple but extensible.

22. **Validate Binary Search Tree (LC98, Medium)**  
    Description: Check if a binary tree is a valid BST.  
    Why frequent: Inorder traversal; common in Google.

23. **Binary Tree Maximum Path Sum (LC124, Hard)**  
    Description: Find max path sum in a binary tree.  
    Why frequent: Recursion with global max; hard for seniors in Amazon.

24. **Lowest Common Ancestor of a Binary Tree (LC236, Medium)**  
    Description: Find LCA of two nodes.  
    Why frequent: Recursive search; frequent in Microsoft.

25. **Kth Smallest Element in a BST (LC230, Medium)**  
    Description: Find kth smallest in BST.  
    Why frequent: Inorder with count; BST properties.

## 6. Graphs
BFS/DFS, cycles, topological sort.

26. **Number of Islands (LC200, Medium)**  
    Description: Count islands in a grid (1s connected).  
    Why frequent: DFS/BFS flood fill; Google favorite.

27. **Course Schedule (LC207, Medium)**  
    Description: Detect if courses can be finished with prerequisites.  
    Why frequent: Topo sort with cycle detect; Amazon for DAGs.

28. **Clone Graph (LC133, Medium)**  
    Description: Deep copy an undirected graph.  
    Why frequent: BFS/DFS with map; tests visited handling.

29. **Pacific Atlantic Water Flow (LC417, Medium)**  
    Description: Find cells where water flows to both oceans.  
    Why frequent: Multi-source BFS; senior for graph traversals.

30. **Word Search (LC79, Medium)**  
    Description: Find if a word exists in a grid.  
    Why frequent: Backtracking on graph; common variant.

## 7. Heaps / Priority Queue
Kth elements, merging, medians.

31. **Kth Largest Element in an Array (LC215, Medium)**  
    Description: Find kth largest using heap.  
    Why frequent: Min-heap of size k; efficient in C++ priority_queue.

32. **Find Median from Data Stream (LC295, Hard)**  
    Description: Add numbers and find median dynamically.  
    Why frequent: Two heaps (max/min); senior design.

33. **Merge K Sorted Lists (LC23, Hard)**  
    Description: Merge k lists using heap.  
    Why frequent: Priority queue for mins; scales to arrays.

34. **Task Scheduler (LC621, Medium)**  
    Description: Schedule tasks with cooldown.  
    Why frequent: Heap for frequencies; practical in Microsoft.

35. **Top K Frequent Elements (LC347, Medium)** (cross-topic)  
    Description: As above, using heap.

## 8. Recursion & Backtracking
Subsets, permutations, puzzles.

36. **Combination Sum (LC39, Medium)**  
    Description: Find combinations summing to target.  
    Why frequent: Backtracking with duplicates; Google.

37. **Subsets (LC78, Medium)**  
    Description: Generate all subsets.  
    Why frequent: Recursive inclusion; powerset problems.

38. **Permutations (LC46, Medium)**  
    Description: Generate all permutations.  
    Why frequent: Backtracking with swaps; common.

39. **Word Break (LC139, Medium)**  
    Description: Break string into dictionary words.  
    Why frequent: Recursion with memo; leads to DP.

40. **N-Queens (LC51, Hard)**  
    Description: Place queens without attacks.  
    Why frequent: Classic backtracking; senior for optimizations.

## 9. Dynamic Programming
Knapsacks, subsequences, paths.

41. **Climbing Stairs (LC70, Easy)**  
    Description: Ways to climb n stairs (1/2 steps).  
    Why frequent: Basic DP fib-like; warmup.

42. **Coin Change (LC322, Medium)**  
    Description: Min coins to make amount.  
    Why frequent: Unbounded knapsack; Amazon.

43. **Longest Increasing Subsequence (LC300, Medium)**  
    Description: Find LIS length.  
    Why frequent: DP O(n^2) or binary search O(n log n); senior variant.

44. **Unique Paths (LC62, Medium)**  
    Description: Paths in grid from top-left to bottom-right.  
    Why frequent: Grid DP; obstacles variant.

45. **House Robber (LC198, Medium)**  
    Description: Max rob without adjacent houses.  
    Why frequent: 1D DP; extends to tree/circle.

## 10. Searching & Sorting
Binary search variants, quickselect.

46. **Search in Rotated Sorted Array (LC33, Medium)**  
    Description: Binary search in rotated array.  
    Why frequent: Modified binary search; Google.

47. **Find Minimum in Rotated Sorted Array (LC153, Medium)**  
    Description: Find min in rotated sorted array.  
    Why frequent: Binary search pivot; common.

48. **Best Time to Buy and Sell Stock (LC121, Easy)**  
    Description: Max profit from one buy/sell.  
    Why frequent: One-pass; variants for multiple transactions.

49. **Merge Sort** (Not LC-specific, implement)  
    Description: Implement merge sort.  
    Why frequent: Stable sort; asked to code in C++ interviews.

50. **Quickselect for Kth Element (LC215 variant)**  
    Description: Find kth smallest using partition.  
    Why frequent: Average O(n); senior for sorting alternatives.

## Bonus Senior-Level Topics
For seniors, expect combos and advanced:
- **LFU Cache (LC460, Hard)**: Design LFU with frequency + recency.
- **Minimum Window Substring (LC76, Hard)**: Sliding window + hash for min substring.
- **Binary Tree Serialize/Deserialize (LC297, Hard)**: Tree to string and back.
- **Trapping Rain Water (LC42, Hard)**: Two pointers or stack for water levels.
- **Word Search II (LC212, Hard)**: Trie + backtracking for multiple words.

This list covers ~80% of common questions. Practice implementing in C++ with optimal time/space. For revision, solve 2-3 per day as suggested.

*(This content is formatted for easy conversion to PDF using tools like Markdown to PDF converters or printing this page. If you need images or further details, let me know.)*
