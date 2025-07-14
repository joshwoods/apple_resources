

- Swift
- FixedWidthInteger
-  &\*(\_:\_:) 

Operator

# &\*(\_:\_:)

Returns the product of the two given values, wrapping the result in case of any overflow.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func &* (lhs: Self, rhs: Self) -> Self
```

**Required** Default implementation provided.

## Parameters 

`lhs`  

The first value to multiply.

`rhs`  

The second value to multiply.

## Discussion

The overflow multiplication operator (`&*`) discards any bits that overflow the fixed width of the integer type. In the following example, the product of `10` and `50` is greater than the maximum representable `Int8` value, so the result is the partial value after discarding the overflowing bits.

```
let x: Int8 = 10 &* 5
// x == 50
let y: Int8 = 10 &* 50
// y == -12 (after overflow)
```

For more about arithmetic with overflow operators, see Overflow Operators in *The Swift Programming Language*.

## Default Implementations

### FixedWidthInteger Implementations

static func &amp;* (Self, Self) -> Self

Returns the product of the two given values, wrapping the result in case of any overflow.

