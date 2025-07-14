

- Swift
- UInt64
-  &-(\_:\_:) 

Operator

# &-(\_:\_:)

Returns the difference of the two given values, wrapping the result in case of any overflow.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func &- (lhs: Self, rhs: Self) -> Self
```

## Parameters 

`lhs`  

A numeric value.

`rhs`  

The value to subtract from `lhs`.

## Discussion

The overflow subtraction operator (`&-`) discards any bits that overflow the fixed width of the integer type. In the following example, the difference of `10` and `21` is less than zero, the minimum representable `UInt` value, so the result is the partial value after discarding the overflowing bits.

```
let x: UInt8 = 21 &- 10
// x == 11
let y: UInt8 = 10 &- 21
// y == 245 (after overflow)
```

For more about arithmetic with overflow operators, see Overflow Operators in *The Swift Programming Language*.

