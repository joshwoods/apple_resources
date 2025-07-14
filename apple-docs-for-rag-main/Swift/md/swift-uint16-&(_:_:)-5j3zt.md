

- Swift
- UInt16
-  &\

Operator

# &\

Returns the result of shifting a value’s binary representation the specified number of digits to the left, masking the shift amount to the type’s bit width.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func & Self
```

## Parameters 

`lhs`  

The value to shift.

`rhs`  

The number of bits to shift `lhs` to the left. If `rhs` is outside the range `0..

## Discussion

Use the masking left shift operator (`&

```
let x: UInt8 = 30                 // 0b00011110
let y = x &

However, if you use `8` as the shift amount, the method first masks the shift amount to zero, and then performs the shift, resulting in no change to the original value.

```
let z = x &

If the bit width of the shifted integer type is a power of two, masking is performed using a bitmask; otherwise, masking is performed using a modulo operation.

