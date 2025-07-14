

- Swift
- BinaryInteger
-  /(\_:\_:) 

Operator

# /(\_:\_:)

Returns the quotient of dividing the first value by the second.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func / (lhs: Self, rhs: Self) -> Self
```

**Required**

## Parameters 

`lhs`  

The value to divide.

`rhs`  

The value to divide `lhs` by. `rhs` must not be zero.

## Discussion

For integer types, any remainder of the division is discarded.

```
let x = 21 / 5
// x == 4
```

## See Also

### Arithmetic

static func + (Self, Self) -> Self

Adds two values and produces their sum.

**Required**

static func - (Self, Self) -> Self

Subtracts one value from another and produces their difference.

**Required**

static func * (Self, Self) -> Self

Multiplies two values and produces their product.

**Required**

