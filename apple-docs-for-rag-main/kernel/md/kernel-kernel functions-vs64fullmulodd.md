

- Kernel
- Kernel Functions
-  vS64FullMulOdd 

Function

# vS64FullMulOdd

Signed 64-bit multiplication; results are twice as wide as multiplicands, odd-numbered elements of multiplicand vectors are used. Note the big-endian convention: the leftmost element is element 0.

macOS 10.0+

``` source
vSInt32 vS64FullMulOdd(vSInt32 vA, vSInt32 vB);
```

