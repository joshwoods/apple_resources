

- Kernel
- Kernel Functions
-  vU64FullMulOdd 

Function

# vU64FullMulOdd

Unsigned 64-bit multiplication; results are twice as wide as multiplicands, odd-numbered elements of multiplicand vectors are used. Note the big-endian convention: the leftmost element is element 0.

macOS 10.0+

``` source
vUInt32 vU64FullMulOdd(vUInt32 vA, vUInt32 vB);
```

