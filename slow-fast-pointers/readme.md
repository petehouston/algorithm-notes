# Slow-Fast Pointers

The technique of using two pointers to keep track and measure data by steps, known as [Floyd's cycle-finding algorithm](https://en.wikipedia.org/wiki/Cycle_detection#Floyd's_Tortoise_and_Hare).

The concept is:

- Using two pointers.
- One pointer, which is moving slowly - **Slow Pointer**, increases step by one unit.
- The other pointer, which is moving fast - **Fast Pointer**, increases steps by two or more units.

**Why using slow-fast pointers?**

- Sometimes, we have an algorithm to track and measure data in a list, but we don't know how far ahead, it might cost us more time and space to complete. Instead, by using slow-fast pointers technique, we can reduce number of steps required so that the algorithm is improved greatly.

## Practice

- [LeetCode 141 - Linked List Cycle](https://leetcode.com/problems/linked-list-cycle/)
- [LeetCode 287 - Find the Duplicate Number](https://leetcode.com/problems/find-the-duplicate-number/)
- [LeetCode 876 - Middle of the Linked List](https://leetcode.com/problems/middle-of-the-linked-list/)

## References:

- [Find Duplicate - by Keith Schwarz](http://keithschwarz.com/interesting/code/?dir=find-duplicate)
- [Cycle Detection - Wikipedia](https://en.wikipedia.org/wiki/Cycle_detection)