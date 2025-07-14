

- Swift
- UInt128
-  /=(\_:\_:) 

Operator

# /=(\_:\_:)

Divides the first value by the second and stores the quotient in the left-hand-side variable.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func /= (a: inout UInt128, b: UInt128)
```

## Discussion

For integer types, any remainder of the division is discarded.

```
var x = 21
x /= 5
// x == 4
```

