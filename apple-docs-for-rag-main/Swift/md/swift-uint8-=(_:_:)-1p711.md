

- Swift
- UInt8
-  \

Operator

# \

Stores the result of shifting a value’s binary representation the specified number of digits to the left in the left-hand-side variable.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func (lhs: inout Self, rhs: Other) where Other : BinaryInteger
```

## Parameters 

`lhs`  

The value to shift.

`rhs`  

The number of bits to shift `lhs` to the left.

## Discussion

The `

```
var x: UInt8 = 30                 // 0b00011110
x 

If you use `11` as `rhs`, `x` is overshifted such that all of its bits are set to zero.

```
var y: UInt8 = 30                 // 0b00011110
y 

Using a negative value as `rhs` is the same as performing a right shift with `abs(rhs)`.

```
var a: UInt8 = 30                 // 0b00011110
a >= 3
// b == 3                         // 0b00000011
```

