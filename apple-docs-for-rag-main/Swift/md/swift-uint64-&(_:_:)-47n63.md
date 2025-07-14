

- Swift
- UInt64
-  &\>\>(\_:\_:) 

Operator

# &\>\>(\_:\_:)

Returns the result of shifting a value’s binary representation the specified number of digits to the right, masking the shift amount to the type’s bit width.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func &>> (lhs: Self, rhs: Other) -> Self where Other : BinaryInteger
```

## Parameters 

`lhs`  

The value to shift.

`rhs`  

The number of bits to shift `lhs` to the right. If `rhs` is outside the range `0..

## Discussion

Use the masking right shift operator (`&>>`) when you need to perform a shift and are sure that the shift amount is in the range `0..

```
let x: UInt8 = 30                 // 0b00011110
let y = x &>> 2
// y == 7                         // 0b00000111
```

However, if you use `8` as the shift amount, the method first masks the shift amount to zero, and then performs the shift, resulting in no change to the original value.

```
let z = x &>> 8
// z == 30                        // 0b00011110
```

If the bit width of the shifted integer type is a power of two, masking is performed using a bitmask; otherwise, masking is performed using a modulo operation.

