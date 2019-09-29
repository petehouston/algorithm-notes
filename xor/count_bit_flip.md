# Count bit-flip

Given two numbers a, b. Determine number of bit flip to convert from a to b.

For example:

```
a = 31, b = 14 => In binary, a = 11111, b = 01110. So it needs to flip the first and last bits to convert. => Return 2.

a = 12, b = 7 => return 3.
```

## Solutions

In linear time, **O(n)**:

```java
int countBitFlip(int a, int b) {
    int x = a ^ b;
    int c = 0;
    while (x > 0) {
        if ((1 & x) > 0) c++;
        x = x >> 1;
    }
    return c;
}
```

## Explanation

Using XOR operation, we know that the same bits will be converted to 0, different bits will be converted to 1.

By doing `a ^ b`, we get a number that contains number of bit 1 that needs to be converted. 

We only need to count number of bit 1 from it.

```
    31 = 11111
XOR
    14 = 01110
--------------
       = 10001
````

There are two bits 1 in result of XOR operation. So count it and return.

