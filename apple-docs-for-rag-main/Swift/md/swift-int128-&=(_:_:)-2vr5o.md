

- Swift
- Int128
-  &\

Operator

# &\

Returns the result of shifting a value’s binary representation the specified number of digits to the left, masking the shift amount to the type’s bit width, and stores the result in the left-hand-side variable.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func &

## Discussion

The `&

```
var x: UInt8 = 30                 // 0b00011110
x &

However, if you pass `19` as `rhs`, the method first bitmasks `rhs` to `3`, and then uses that masked value as the number of bits to shift `lhs`.

```
var y: UInt8 = 30                 // 0b00011110
y &

