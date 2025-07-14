

- Swift
- Int
-  -=(\_:\_:) 

Operator

# -=(\_:\_:)

Subtracts the second value from the first and stores the difference in the left-hand-side variable.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func -= (lhs: inout Int, rhs: Int)
```

## Parameters 

`lhs`  

A numeric value.

`rhs`  

The value to subtract from `lhs`.

## Discussion

The difference of the two arguments must be representable in the arguments’ type. In the following example, the result of `21 - 50` is less than zero, the minimum representable `UInt8` value:

```
var x: UInt8 = 21
x -= 50
// Overflow error
```

Note

Overflow checking is not performed in `-Ounchecked` builds.

