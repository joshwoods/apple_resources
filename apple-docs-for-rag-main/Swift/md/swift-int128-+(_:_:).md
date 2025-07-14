

- Swift
- Int128
-  +(\_:\_:) 

Operator

# +(\_:\_:)

Adds two values and produces their sum.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func + (a: Int128, b: Int128) -> Int128
```

## Discussion

The addition operator (`+`) calculates the sum of its two arguments. For example:

```
1 + 2                   // 3
-10 + 15                // 5
-15 + -5                // -20
21.5 + 3.25             // 24.75
```

You cannot use `+` with arguments of different types. To add values of different types, convert one of the values to the other value’s type.

```
let x: Int8 = 21
let y: Int = 1000000
Int(x) + y              // 1000021
```

