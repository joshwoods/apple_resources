

- Swift
- Int128
-  leadingZeroBitCount 

Instance Property

# leadingZeroBitCount

The number of leading zeros in this value’s binary representation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var leadingZeroBitCount: Int { get }
```

## Discussion

For example, in a fixed-width integer type with a `bitWidth` value of 8, the number *31* has three leading zeros.

```
let x: Int8 = 0b0001_1111
// x == 31
// x.leadingZeroBitCount == 3
```

If the value is zero, then `leadingZeroBitCount` is equal to `bitWidth`.

