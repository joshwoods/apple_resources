

- Swift
- Numeric
-  \*(\_:\_:) 

Operator

# \*(\_:\_:)

Multiplies two values and produces their product.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func * (lhs: Self, rhs: Self) -> Self
```

**Required**

## Parameters 

`lhs`  

The first value to multiply.

`rhs`  

The second value to multiply.

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

