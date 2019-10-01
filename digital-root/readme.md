# Digital Root

The digital root (also repeated digital sum) of a non-negative integer is the (single digit) value obtained by an iterative process of summing digits, on each iteration using the result from the previous iteration to compute a digit sum. The process continues until a single-digit number is reached.

For example, the digital root of 65,536 is 7, because 6 + 5 + 5 + 3 + 6 = 25 and 2 + 5 = 7.

Digital roots can be calculated with congruences in modular arithmetic rather than by adding up all the digits, a procedure that can save time in the case of very large numbers.

Digital roots can be used as a sort of checksum, to check that a sum has been performed correctly. If it has, then the digital root of the sum of the given numbers will equal the digital root of the sum of the digital roots of the given numbers. This check, which involves only single-digit calculations, can catch many errors in calculation.

Digital roots are used in Western numerology, but certain numbers deemed to have occult significance (such as 11 and 22) are not always completely reduced to a single digit.

The number of times the digits must be summed to reach the digital root is called a number's additive persistence; in the above example, the additive persistence of 65,536 is 2.

The formula of calculating the Digital Root:

```
dr(n) = 1 + ((n - 1) mod 9)
```

## Practice 

- [LeetCode 258 - Add Digits](https://leetcode.com/problems/add-digits/)

## References

- [Digital Root - Wikipedia](https://en.wikipedia.org/wiki/Digital_root)