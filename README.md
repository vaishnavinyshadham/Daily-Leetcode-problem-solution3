# Daily-Leetcode-problem-solution3

PROBLEM

Given two strings s and part, perform the following operation on s until all occurrences of the substring part are removed:
Find the leftmost occurrence of the substring part and remove it from s.
Return s after removing all occurrences of part.
A substring is a contiguous sequence of characters in a string.

Intuition

Repeatedly removes the leftmost occurrence of part from s until no more occurrences are found.
Edge Cases Considered:
When part is not found in s, return s as-is.
If part completely removes s, return an empty string "".
If s or part is an empty string, return s

Approach

Use the find() function to locate the first occurrence of part in s.
Use erase() to remove the found substring.
Repeat the process until find() returns string::npos, meaning part no longer exists in s.

Complexity

Time complexity:
O(N * M) in the worst case, where:
N is the length of s.
M is the length of part.
This is because find() runs in O(N) and erase() in O(N), leading to a worst-case of O(N * M) if part appears frequently.

Space complexity:
O(1)

 
