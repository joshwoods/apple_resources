

- Swift
- AdditiveArithmetic
-  -(\_:\_:) 

Operator

# -(\_:\_:)

Subtracts one value from another and produces their difference.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func - (lhs: Self, rhs: Self) -> Self
```

**Required**

## Parameters 

`lhs`  

A numeric value.

`rhs`  

The value to subtract from `lhs`.

## Discussion

The subtraction operator (`-`) calculates the difference of its two arguments. For example:

```
8 - 3                   // 5
-10 - 5                 // -15
100 - -5                // 105
10.5 - 100.0            // -89.5
```

You cannot use `-` with arguments of different types. To subtract values of different types, convert one of the values to the other value’s type.

```
let x: UInt8 = 21
let y: UInt = 1000000
y - UInt(x)             // 999979
```

