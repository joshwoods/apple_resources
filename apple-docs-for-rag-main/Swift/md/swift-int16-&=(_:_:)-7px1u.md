

- Swift
- Int16
-  &\>\>=(\_:\_:) 

Operator

# &\>\>=(\_:\_:)

Calculates the result of shifting a value’s binary representation the specified number of digits to the right, masking the shift amount to the type’s bit width, and stores the result in the left-hand-side variable.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func &>>= (lhs: inout Self, rhs: Other) where Other : BinaryInteger
```

## Parameters 

`lhs`  

The value to shift.

`rhs`  

The number of bits to shift `lhs` to the right. If `rhs` is outside the range `0..

## Discussion

The `&>>=` operator performs a *masking shift*, where the value passed as `rhs` is masked to produce a value in the range `0..

```
var x: UInt8 = 30                 // 0b00011110
x &>>= 2
// x == 7                         // 0b00000111
```

However, if you use `19` as `rhs`, the operation first bitmasks `rhs` to `3`, and then uses that masked value as the number of bits to shift `lhs`.

```
var y: UInt8 = 30                 // 0b00011110
y &>>= 19
// y == 3                         // 0b00000011
```

