

- Swift
- UInt16
-  &+(\_:\_:) 

Operator

# &+(\_:\_:)

Returns the sum of the two given values, wrapping the result in case of any overflow.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func &+ (lhs: Self, rhs: Self) -> Self
```

## Parameters 

`lhs`  

The first value to add.

`rhs`  

The second value to add.

## Discussion

The overflow addition operator (`&+`) discards any bits that overflow the fixed width of the integer type. In the following example, the sum of `100` and `121` is greater than the maximum representable `Int8` value, so the result is the partial value after discarding the overflowing bits.

```
let x: Int8 = 10 &+ 21
// x == 31
let y: Int8 = 100 &+ 121
// y == -35 (after overflow)
```

For more about arithmetic with overflow operators, see Overflow Operators in *The Swift Programming Language*.

