

- Swift
- UInt128
-  &\

Operator

# &\

Returns the result of shifting a value’s binary representation the specified number of digits to the left, masking the shift amount to the type’s bit width, and stores the result in the left-hand-side variable.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func &(lhs: inout Self, rhs: Other) where Other : BinaryInteger
```

## Parameters 

`lhs`  

The value to shift.

`rhs`  

The number of bits to shift `lhs` to the left. If `rhs` is outside the range `0..

## Discussion

The `&

```
var x: UInt8 = 30                 // 0b00011110
x &

However, if you pass `19` as `rhs`, the method first bitmasks `rhs` to `3`, and then uses that masked value as the number of bits to shift `lhs`.

```
var y: UInt8 = 30                 // 0b00011110
y &

