

- Swift
- Int16
-  leadingZeroBitCount 

Instance Property

# leadingZeroBitCount

The number of leading zeros in this value’s binary representation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

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

