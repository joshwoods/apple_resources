

- Swift
- Duration
-  +(\_:\_:) 

Operator

# +(\_:\_:)

Adds two values and produces their sum.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func + (lhs: Duration, rhs: Duration) -> Duration
```

## Parameters 

`lhs`  

The first value to add.

`rhs`  

The second value to add.

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

