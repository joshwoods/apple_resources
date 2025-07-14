

- Swift
- Int128
-  \*(\_:\_:) 

Operator

# \*(\_:\_:)

Multiplies two values and produces their product.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func * (a: Int128, b: Int128) -> Int128
```

## Discussion

The multiplication operator (`*`) calculates the product of its two arguments. For example:

```
2 * 3                   // 6
100 * 21                // 2100
-10 * 15                // -150
3.5 * 2.25              // 7.875
```

You cannot use `*` with arguments of different types. To multiply values of different types, convert one of the values to the other value’s type.

```
let x: Int8 = 21
let y: Int = 1000000
Int(x) * y              // 21000000
```

