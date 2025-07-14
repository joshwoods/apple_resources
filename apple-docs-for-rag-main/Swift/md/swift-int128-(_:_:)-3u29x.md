

- Swift
- Int128
-  /(\_:\_:) 

Operator

# /(\_:\_:)

Returns the quotient of dividing the first value by the second.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func / (a: Int128, b: Int128) -> Int128
```

## Discussion

For integer types, any remainder of the division is discarded.

```
let x = 21 / 5
// x == 4
```

