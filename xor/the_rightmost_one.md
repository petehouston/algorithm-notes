# The rightmost 1

Given a number, return the rightmost 1 of its binary representation.

Examples:

```
11 => In binary: 11 = 1011 => Return 0001.
10 => In binary: 10 = 1010 => Return 0010.
```

## Solutions

In constant time, **O(1)**.

```java
int rightmostOne(int n) {
	return n ^ (n & (n - 1));
}
```

## Explanation

The trick here is to leverage to properties of AND and XOR.

- in AND, the same bits are kept.
- in XOR, the same bits become 0, the different bits become 1.

We notice that **n** and **n - 1** differs only in one bit adding. Hence, we need to find the last bit-flip from 0 to 1 to get **n - 1** to become **n**, and that's done!

```
0111 + 0001 = 1000 => n = 1000 => returns 1000
0011 + 0001 = 0100 => n = 0100 => returns 0100
1010 + 0001 = 1011 => n = 1011 => returns 0010
```