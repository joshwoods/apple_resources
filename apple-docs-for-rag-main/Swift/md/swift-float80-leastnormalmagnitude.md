

- Swift
- Float80
-  leastNormalMagnitude 

Type Property

# leastNormalMagnitude

The least positive normal number.

macOS 10.10+

``` source
static var leastNormalMagnitude: Float80 { get }
```

## Discussion

This value compares less than or equal to all positive normal numbers. There may be smaller positive numbers, but they are *subnormal*, meaning that they are represented with less precision than normal numbers.

This value corresponds to type-specific C macros such as `FLT_MIN` and `DBL_MIN`. The naming of those macros is slightly misleading, because subnormals, zeros, and negative numbers are smaller than this value.

