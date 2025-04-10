---
layout: Binary Search Popcorn Hacks
title: Binary Search Popcorn Hacks
search_exclude: true
permalink: /search/
---

## Popcorn Hack 1
Popcorn Hack 1 (from CB MC 2020)
The procedure BinarySearch(numList, target) correctly implements a binary search algorithm on the list of numbers numList. The procedure returns an index here target occurs in numList, or -1 if target does not occur in numList.

Which of the following conditions must be met in order for the procedure to work as intended? Explain why.

a) The length of numList must be even
b) The list numList must not contain any duplicate values
c) The values in numList must be in sorted order
d) The value of target must not be equal to -1

## Answer: c) The values in numList must be in sorted order
✅ Explanation:
Binary search is an efficient algorithm that works by repeatedly dividing a sorted list in half to find the target value. For this method to work as intended, the list must be in sorted order (either ascending or descending, though usually ascending).

## Popcorn Hack 2
Which of the following statements correctly describes a disadvantage of binary search compared to linear search? Explain why your answer is correct and why the others are wrong.

a) Binary search takes more time on average than linear search  
b) Binary search cannot be used on unsorted lists without modifications  
c) Binary search always returns the first occurrence of the target  
d) Binary search can only be used on lists with unique values  

answer: b) Binary search cannot be used on unsorted lists without modifications
✅ Explanation:
Binary search is only effective on sorted lists. If the list is unsorted, binary search can't make correct decisions about which half to eliminate during the search. So unless you sort the list first, binary search won’t work properly.

❌ Why the other options are wrong:
a) Binary search takes more time on average than linear search
→ False. Binary search is actually faster on average for large, sorted datasets — it runs in O(log n) time, while linear search takes O(n) time.

c) Binary search always returns the first occurrence of the target
→ False. Binary search finds an occurrence, but not necessarily the first. You would need to modify it if you specifically want the first occurrence.

d) Binary search can only be used on lists with unique values
→ False. Binary search works with duplicates; it just returns one of the matching indices.

