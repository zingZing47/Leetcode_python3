# (1) Arrays & Hashing

| No.           | Name             | Num solutions| Descriptions| Functions|
| ------------- | -----------------| -------------| -----------------| -------------|
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



# (0) Others

| No.           | Name             | Num solutions| Descriptions     |Functions     |
| ------------- | -----------------| -------------| -----------------| -------------|
| 45           | Jump Game II    | 1            |Greedy| - |
| 172            | Factorial Trailing Zeroes    | 1    |the number of factorial trailing 0 = //5| - |




1. List (No.2, 21, 23 141, 142, 876, 19, 160, 206, 92, 25, 234)
2. Array (No. 26, 83, 27, 283, 167, 344, 5)
3. Binary Tree
4. Graph
5. Data Structure
