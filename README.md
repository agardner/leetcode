# My Python Solutions for Leetcode

[The whole lists](https://github.com/qiyuangong/leetcode/tree/master/python):

&hearts; means you need a subscription.

| # | Title | Solution | Basic idea (One line) |
|---| ----- | -------- | --------------------- |
| 1 | [Two Sum](https://leetcode.com/problems/two-sum/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/1_Two_Sum.py) | 1. Hash O(n) and O(n) space<br>2. Sort and search with two points O(n) and O(1) space |
| 2 | [Add Two Numbers](https://leetcode.com/problems/add-two-numbers/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/2_Add_Two_Numbers.py) | Note the carry from lower digit. |
| 3 | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/3_Longest_Substring_Without_Repeating_Characters.py) |1. Check every possible substring O(n^2) <br>2. Remember the character index and current check pos, if character index >= current pos, then there is duplicate |
| 5 | [Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/5_Longest_Palindromic_Substring.py) | [Background knowledge](http://en.wikipedia.org/wiki/Longest_palindromic_substring)<br>1. DP if s[i]==s[j] and P[i+1, j-1] then P[i,j]<br>2. A palindrome can be expanded from its center<br>3. Manacher algorithm|
| 7 | [Reverse Integer](https://leetcode.com/problems/reverse-integer/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/7_Reverse_Integer.py) | Overflow when the result is greater than 2147483647
| 8 | [String to Integer (atoi)](https://leetcode.com/problems/string-to-integer-atoi/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/8_String_to_Integer(atoi).py) | Overflow, Space, and negative number |
| 9 | [Palindrome Number](https://leetcode.com/problems/palindrome-number/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/9_Palindrome_Number.py)| Get the len and check left and right with 10^len, 10 |
| 12 | [Integer to Roman](https://leetcode.com/problems/integer-to-roman/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/12_Integer_to_Roman.py) | [Background knowledge](http://www.rapidtables.com/convert/number/how-number-to-roman-numerals.htm) Just like 10-digit number, divide and minus |
| 13 | [Roman to Integer](https://leetcode.com/problems/roman-to-integer/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/13_Roman_to_Integer.py) | Add all curr, if curr > prev, then need to subtract 2 * prev |
| 15 | [3Sum](https://leetcode.com/problems/3sum/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/15_3Sum.py) | 1. Sort and O(n^2) search with three points <br>2. Multiple Two Sum (Problem 1) |
| 16 | [3Sum Closest](https://leetcode.com/problems/3sum-closest/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/16_3Sum_Closest.py) | Sort and Multiple Two Sum check abs|
| 18 | [4Sum](https://leetcode.com/problems/4sum/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/18_4Sum.py) | The same as 3Sum, but we can merge pairs with the same sum |
| 20 | [Valid Parentheses](https://leetcode.com/problems/valid-parentheses/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/20_Valid_Parentheses.py) | 1. Stack<br>2. Replace all parentheses with '', if empty then True |
| 21 | [Merge Two Sorted Lists](https://leetcode.com/problems/merge-two-sorted-lists/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/21_Merge_Two_Sorted_Lists.py) | Add a dummy head, then merge two sorted list in O(m+n) |
| 23 | [Merge k Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/23_Merge_k_Sorted_Lists.py) | 1. Priority queue O(nk log k)<br>2. Binary merge O(nk log k)|  |
| 24 | [Swap Nodes in Pairs](https://leetcode.com/problems/swap-nodes-in-pairs/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/24_Swap_Nodes_in_Pairs.py) | Add a dummy and store the prev |
| 28 | [Implement strStr()](https://leetcode.com/problems/implement-strstr/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/28_Implement_strStr().py) | 1. O(nm) comparison <br>2. KMP |
| 35 | [Search Insert Position](https://leetcode.com/problems/search-insert-position/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/35_Search_Insert_Position.py) | Binary Search |
| 53 | [Maximum Subarray](https://leetcode.com/problems/maximum-subarray/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/53_Maximum_Subarray.py) | 1. Recursion, O(nlgn), O(lgn)<br> 2. Bottom-up DP, O(n) and O(n)<br>3. Bottom-up DP, f(x) = max(f(x-1)+A[x], A[x]), f(x) = max(f(x-1)+A[x], A[x]),O(n) and O(1) |
| 54 | [Spiral Matrix](https://leetcode.com/problems/spiral-matrix/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/54_Spiral_Matrix.py) | O(nm) 1. Turn in the corner and loop<br>2. (0, 1) -> (1, 0) -> (0, -1) -> (-1, 0) |
| 62 | [Unique Paths](https://leetcode.com/problems/unique-paths/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/62_Unique_Paths.py) | 1. Bottom-up DP, dp[i][j] = dmap[i-1][j] + dmap[i][j-1], O(mn) and O(mn)<br>2. Combination (m+n-2, m-1) |
| 63 | [Unique Paths II](https://leetcode.com/problems/unique-paths-ii/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/63_Unique_Paths_II.py) | Bottom-up DP, dp[i][j] = dmap[i-1][j] + dmap[i][j-1] (if block, then 0), O(mn) and O(mn) |
| 65 | [Valid Number](https://leetcode.com/problems/valid-number/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/65_Valid_Number.py) | 1. strip leading and tailing space, then check float using exception, check e using split <br>2. check is number split by . or e, note that number after e may be negative |
| 66 | [Plus One](https://leetcode.com/problems/plus-one/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/66_Plus_One.py) | Check if current digit == 9. |
| 70 | [Climbing Stairs](https://leetcode.com/problems/climbing-stairs/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/70_Climbing_Stairs.py) | Bottom-up DP, dp[i] = dp[i - 2] + dp[i- 1] <br>1. O(n) and O(n)<br>2. Only two variables are needed, O(n) and O(1) |
| 72 | [Edit Distance](https://leetcode.com/problems/edit-distance/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/72_Edit_Distance.py) | [Background](https://en.wikipedia.org/wiki/Edit_distance)<br> 1. DP O(n^2) space<br>2. DP O(n) space |
| 98 | [Validate Binary Search Tree](https://leetcode.com/problems/validate-binary-search-tree/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/98_Validate_Binary_Search_Tree.py) | 1. Stack O(n) and O(n)<br>2. Recursion O(n) and O(n) |
| 104 | [Maximum Depth of Binary Tree](https://leetcode.com/problems/maximum-depth-of-binary-tree/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/104_Maximum_Depth_of_Binary_Tree.py)| Recursion max(left, right) + 1 |
| 108 | [Convert Sorted Array to Binary Search Tree](https://leetcode.com/problems/convert-sorted-array-to-binary-search-tree/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/108_Convert_Sorted_Array_to_Binary_Search_Tree.py)| Recursion O(n) and O(nlgn)|
| 109 | [Convert Sorted List to Binary Search Tree](https://leetcode.com/problems/convert-sorted-list-to-binary-search-tree/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/109_Convert_Sorted_List_to_Binary_Search_Tree.py) | 1. Two points fast (next next) and slow (next) O(nlgn) and O(n)<br>2. Bottom-up recursion O(n) and O(lgn) |
| 110 | [Balanced Binary Tree](https://leetcode.com/problems/balanced-binary-tree/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/110_Balanced_Binary_Tree.py) | Recursion 1. Top-down O(n^2) and O(n), Bottom-up recursion with sentinel -1 O(n) and O(n) |
| 111 | [Minimum Depth of Binary Tree](https://leetcode.com/problems/minimum-depth-of-binary-tree/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/111_Minimum_Depth_of_Binary_Tree.py) | 1. Recursion, note that when size of left (ld) or right (rd) is 0, then min = 1 + ld + rd<br> 2. BFS check by level (right most), which is much faster than recursion |
| 124 | [Binary Tree Maximum Path Sum](https://leetcode.com/problems/binary-tree-maximum-path-sum/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/124. Binary Tree Maximum Path Sum.py) | Recursion O(n) and O(n), max (left + node, right + node, left + node + right) |
| 125 | [Valid Palindrome](https://leetcode.com/problems/valid-palindrome/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/125_Valid_Palindrome.py)| Exclude non-alphanumeric characters and compare O(n) |
| 128 | [Longest Consecutive Sequence](https://leetcode.com/problems/longest-consecutive-sequence/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/128_Longest_Consecutive_Sequence.py) | Set or hash, pop adjacency, O(n) and O(n) |
| 133 | [Clone Graph](https://leetcode.com/problems/clone-graph/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/133_Clone_Graph.py) | Hash and DFS or BFS |
| 136 | [Single Number](https://leetcode.com/problems/single-number/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/136_Single_Number.py) | 1. Hash or set, O(n) and O(n)<br>2. xor O(n) and O(1) |
| 137 | [Single Number II](https://leetcode.com/problems/single-number-ii/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/137_Single_Number_II.py) | 1. ctypes 32 % 3 and &, O(n) and O(1)<br>2. ones, twos, threes as bitmask (e.g. ones represents ith bit had appeared once), O(n) and O(1) | 
| 138 | [Copy List with Random Pointer](https://leetcode.com/problems/copy-list-with-random-pointer/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/138_Copy_List_with_Random_Pointer.py) | 1. Hash O(n) and O(n)<br>2.  Modify original structure: Original->Copy->Original, then node.next.random = node.random.next, O(n) and O(1) |
| 141 | [Linked List Cycle](https://leetcode.com/problems/linked-list-cycle/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/.py) | 1. Hash or set<br> 2. Two points (fast and slow)<br>3. Add a max and check if reach the max |
| 142 | [Linked List Cycle II](https://discuss.leetcode.com/topic/2975/o-n-solution-by-using-two-pointers-without-change-anything) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/142_Linked_List_Cycle_II.py) | Two points, a+b=nr |
| 143 | [Reorder List](https://leetcode.com/problems/reorder-list/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/143_Reorder_List.py) | 1. List as index to rebuild relation, O(n) and O(n)<br>2. Two points, O(n) and O(1) |
| 144 | [Binary Tree Preorder Traversal](https://leetcode.com/problems/binary-tree-preorder-traversal/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/144_Binary_Tree_Preorder_Traversal.py) | 1. Recursion, O(n) and O(n)<br>2. Stack, O(n) and O(n) |
| 145 | [Binary Tree Postorder Traversal](https://leetcode.com/problems/binary-tree-postorder-traversal/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/145_Binary_Tree_Postorder_Traversal.py) | 1. Recursion, O(n) and O(n)<br>2. Stack, O(n) and O(n)  |
| 146 | [LRU Cache](https://leetcode.com/problems/lru-cache/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/146_LRU_Cache.py) | 1. Queue and dict<br>2. OrderedDict |
| 150 | [Evaluate Reverse Polish Notation](https://leetcode.com/problems/evaluate-reverse-polish-notation/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/150_Evaluate_Reverse_Polish_Notation.py) | Stack |
| 151 | [Reverse Words in a String](https://discuss.leetcode.com/category/159/reverse-words-in-a-string) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/151_Reverse_Words_in_a_String.py)| 1. Python split by space <br>2. Reverse all and reverse words |
| 152 | [Maximum Product Subarray](https://leetcode.com/problems/maximum-product-subarray/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/152_Maximum_Product_Subarray.py) | DP, f(k) = max(f(k-1) * A[k], A[k], g(k-1) * A[k]), g(k) = min(g(k-1) * A[k], A[k], f(k-1) * A[k]), O(n) and O(1) |
| 153 | [Find Minimum in Rotated Sorted Array](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/153_Find_Minimum_in_Rotated_Sorted_Array.py) | Binary search with conditions, A[l] > A[r] |
| 154 | [Find Minimum in Rotated Sorted Array II](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array-ii/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/154_Find_Minimum_in_Rotated_Sorted_Array_II.py) | Binary search with conditions, A[l] > A[r], A[l]=A[mid]=A[r] |
| 155 | [Min Stack](https://leetcode.com/problems/min-stack/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/155_Min_Stack.py) | Add another stack for min stack, maintance this stack when the main stack pop or push |
| 156 | [Binary Tree Upside Down](https://leetcode.com/problems/binary-tree-upside-down/) &hearts;| [Python](https://github.com/qiyuangong/leetcode/blob/master/python/156_Binary_Tree_Upside_Down.py) | p.left = parent.right, parent.right = p.right, p.right = parent, parent = p.left, p = left |
| 157	| [Read N Characters Given Read4](https://leetcode.com/problems/read-n-characters-given-read4/) &hearts; | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/157_Read_N_Characters_Given_Read4.py) | Handle the edge case (the end) |
| 158 | [Read N Characters Given Read4 II - Call multiple times](https://leetcode.com/problems/read-n-characters-given-read4-ii-call-multiple-times/) &hearts;| [Python](https://github.com/qiyuangong/leetcode/blob/master/python/158_Read_N_Characters_Given_Read4_II_Call_multiple_times.py) | Store the pos and offset that is read by last read4 |
| 159 | [Longest Substring with At Most Two Distinct Characters](https://leetcode.com/problems/longest-substring-with-at-most-two-distinct-characters/) &hearts; | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/159_Longest_Substring_with_At_Most_Two_Distinct_Characters.py) | Maintain a sliding window that always satisfies such condition |
| 161 | [One Edit Distance](https://leetcode.com/problems/one-edit-distance/) &hearts;| [Python](https://github.com/qiyuangong/leetcode/blob/master/python/161_One_Edit_Distance.py) | 1. Check the different position and conditions<br>2. [Edit distance](https://leetcode.com/problems/edit-distance/)|
| 163 | [Missing Ranges](https://leetcode.com/problems/missing-ranges/) &hearts; | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/163_Missing_Ranges.py) | Add -1 to lower for special case, then check if curr - prev >= 2|
| 166 | [Fraction to Recurring Decimal](https://leetcode.com/problems/fraction-to-recurring-decimal/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/166_Fraction_to_Recurring_Decimal.py) | % and Hash to find duplicate |
| 167 | [Two Sum II - Input array is sorted](https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/) | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/167_Two_Sum_II_Input_array_is_sorted.py) | Two points O(n) and O(1) |
| 186 | [Reverse Words in a String II](https://leetcode.com/problems/reverse-words-in-a-string-ii/) &hearts;| [Python](https://github.com/qiyuangong/leetcode/blob/master/python/186_Reverse_Words_in_a_String_II.py) | Reverse all and reverse each words |
| 340 | [Longest Substring with At Most K Distinct Characters](https://leetcode.com/problems/longest-substring-with-at-most-k-distinct-characters/) &hearts; | [Python](https://github.com/qiyuangong/leetcode/blob/master/python/340_Longest_Substring_with_At_Most_K_Distinct_Characters.py) | Maintain a sliding window with at most k distinct characters and a count for this window. Note that the start position need a loop to update.|