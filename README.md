# (1) Arrays & Hashing

| No.           | Name             | Num solutions| Descriptions| Functions|
| ------------- | -----------------| -------------| -----------------| -------------|
| 1           | Two Sum| 1 | HashMap  | `enumerate()`,`preMap = {}`|
| 36           | Valid Sudoku| 1 | DefaultDictionary  | `defaultdict()`, `board[r][c]`|
| 49           | Group Anagram| 1 | DefaultDictionary  | `defaultdict()`, `tuple()`,`count = [0] * 26`|
| 128           |Longest Consecutive Sequence| 1 | set, length = y-n  | `set()`|
| 217           | Contains Duplicate| 4 | Hashset  | `sort()`, `set()`|
| 238           | Product of Array Except Self| 2 | -  | -|
| 242           | Valid Anagram| 3 | HashMap  | `enumerate()`, `counter()`|
| 271           | Encode and Decode Strings| 1 | Record the length of each string  | str(len(i)) + "#" + i|
| 347           | Top K Frequent Elements| 1 | HashMap+Array  | `get()`, `items()`|
| 659           | Split Array into Consecutive Subsequences| 1 | Hashmap | `collections.Counter()` or `defaultdict(int)`|



# (2) Two pointers

| No.           | Name             | Num solutions| Descriptions     |Functions     |
| ------------- | -----------------| -------------| -----------------| -------------|
| 11            | Container With Most Water | 1            | 2 pointers: Move the smaller one| - |
| 15            | 3Sum             | 1            | 2 pointers + HashMap| `sort()`, `enumerate()`, `append()` |
| 42            | Trapping Rain Water| 1          | 2 pointers:similar to No.11  | - |
| 125           | Valid Palindrome | 2            | 2 pointers       | `isalnum()` |
| 1470           | Shuffle the Array | 1            | 2 pointers       | - |


# (3) Sliding Window

| No.           | Name                              | Num solutions| Descriptions     |Functions     |
| ------------- | -------------------------------| -------------| -----------------| -------------|
| 3             |Longest Substring Without Repeating Characters| 1   | 2 pointers + set: use while not if | charset = `set()` |
| 121            |Best Time to Buy and Sell Stock| 1            | 2 pointers l=r    | - |
| 424         |Longest Repeating Character Replacement| 1   | 2 pointers + HashMap | count.get(s[r], 0)|
| 567         |Permutation in String| 1   | 2 pointers + index | `ord()`, `[0]* 26`|




# (4) Stack

| No.     | Name             | Num solutions| Descriptions| Functions|
| --------| -----------------| -------------| -----------------| -------------|
| 20      | Valid Parentheses| 1            | Hashmap+Stack  | `stack = []`, `pop()`, `append()`|
| 22      | Generate Parentheses| 1         | Stack+function  | `stack = []`|
| 150     | Evaluate Reverse Polish Notation   | 1  | Stack  |  `pop()`, `append()`, 5 cases|
| 155     | Min Stack        | 1            | 2* Stack  | `self.stack = []`, `pop()`, `append()`|
| 739     | Daily Temperatures  | 1         | stack((t,i))  |  `res[stackC] = i - stackC`, `enumerate()`|





# (5) Binary Search

| No.     | Name             | Num solutions| Descriptions     | Functions|
| --------| -----------------| -------------| -----------------| -------------|
| 33      | Search in Rotated Sorted Array| 1   | 2 sorted arrays | `if nums[l] <= nums[m]` on the left portion |
| 34      | Find First and Last Position of Element in Sorted Array| 1   | rightMargin & leftMargin | `nums[r] == target`keep searching|
| 74      | Search a 2D Matrix    | 2   | newArray or ChooseRow | `ows, cols = len(matrix), len(matrix[0])`|
| 704     | Binary Search    | 1            | 2 Pointer        | `while l <= r`, `m = l + (r-l)// 2`|
| 875     | Koko Eating Bananas    | 1      | leftMargin       | `if totalTime <= h: k=m r=m-1`, `math.ceil() & //`|
| StoO 53 | Finding Numbers in Sorted Arrays I   | 1   | rightMargin & leftMargin: !return potiner  | length= rs - ls + 1|




# (6) Linked List

| No.     | Name             | Num solutions| Descriptions     | Functions|
| --------| -----------------| -------------| -----------------| -------------|
| 2       |  Add Two Numbers | 1   | carry = val // 10 | `v1 = l1.val if l1 else 0`, `l1 = l1.next if l1 else None`|
| 19       |  Remove Nth Node From End of List  |1   | reverse or locate the target node with l&r | `dummy = ListNode(0,head)`|
| 138      | Copy List with Random Pointer  |1   | hashmap: copy and link nodes | `copy = Node(cur.val)`|
| 141      | Linked List Cycle |1   | fast&slow pointers | `dummy = ListNode(0,head)`|
| 143      |  Reorder List | 1   | Medium, reverse+merge | - |
| 287      |  Find the Duplicate Number | 1   | LIST, Floyd's : Cycle, fast+slow & slow+slow2 | `fast = nums[nums[fast]]` |




# (7) Trees

| No.     | Name             | Num solutions| Descriptions     | Functions|
| --------| -----------------| -------------| -----------------| -------------|
| 98     |  Validate Binary Search Tree | 1   | iterate DFS | `float("-inf")`|
| 100     |  Same Tree | 1   | reverse | `self.isSameTree(p.left, q.left)`|
| 102     |  Binary Tree Level Order Traversal | 1   | BFS | `collections.deque()`|
| 104     |  Maximum Depth of Binary Tree | 3  | Good question to learn DFS, BFS | `stack[]`,`deque()`,`append()`on the right of queue,`q.popleft()`|
| 105     | Construct Binary Tree from Preorder and Inorder Traversal | 1   | building a tree basded on preorder and inorder | `mid = inorder.index(preorder[0])`|
| 107     |  Binary Tree Level Order Traversal II | 1   | iterate + reverse | `res[::-1]`|
| 110     |  Balanced Binary Tree | 1 recursive DFS| [bool, height] | - |
| 226     |  Invert Binary Tree | 1         | Switch right and left | `self.invertTree()`|
| 230     |  Kth Smallest Element in a BST | 1         | Switch right and left | `self.invertTree()`|
| 235     |  Lowest Common Ancestor of a Binary Search Tree | 1         | iterative | frist left then right|
| 572     |  Subtree of Another Tree | 1         | Check same tree? subtree? | `self.isSameTree()`|
| 543     |  Diameter of Binary Tree | 1   | Start form bottom, update height+diameter | |
| 1448     | Count Good Nodes in Binary Tree | 1   | DFS |`res = 1 if node.val >= maxVal else 0` |



# (8) Heap

| No.     | Name             | Num solutions| Descriptions     | Functions|
| --------| -----------------| -------------| -----------------| -------------|
| 703     |  Kth Largest Element in a Stream | 1   | MinHeap, pop the smallest value -> return minHeap[0] | `heapq.heapify()`|


`heapq.heappop()`: Pop and return the smallest item from the heap

`heapq.heappush()`: Push the value item onto the heap

`heapq.heapify(x)`: Transform list x into a heap, in-place, in linear time.


# (0) Others

| No.           | Name             | Num solutions| Descriptions     |Functions     |
| ------------- | -----------------| -------------| -----------------| -------------|
| 9            | Palindrome Number | 3            |String            | invert = invert*10 + n//10 |
| 45           | Jump Game II      | 1            |Greedy| - |
| 172            | Factorial Trailing Zeroes    | 1    |the number of factorial trailing 0 = //5| - |
| 692            | Top K Frequent Words   | 1    |Samilar to 347| `collections.Counter()`, `sorted(list, key=lamda x:(-cnt[x], x))[:k]` |
| 208            | Implement Trie (Prefix Tree)   | 1    |Trie| `TrieNode()` |




# Data Structures
## Deque
· Doubly Ended Queue, suitable when need quicker append and pop operations from both the ends of the container. 

  Time: O(1) for pop and append operations
  
  `index(ele, beg, end)`, `insert(i, a)` a is the element, i is the position, `remove()`removes the first occurrence of the selected value
  
  `append()` add on the right, `appendleft()`; `pop()` remove from the left, `popleft()`
