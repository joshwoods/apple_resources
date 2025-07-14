

- Swift
- Int
-  &=(\_:\_:) 

Operator

# &=(\_:\_:)

Stores the result of performing a bitwise AND operation on the two given values in the left-hand-side variable.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func &= (lhs: inout Int, rhs: Int)
```

## Parameters 

`lhs`  

An integer value.

`rhs`  

Another integer value.

## Discussion

A bitwise AND operation results in a value that has each bit set to `1` where *both* of its arguments have that bit set to `1`. For example:

```
var x: UInt8 = 5          // 0b00000101
let y: UInt8 = 14         // 0b00001110
x &= y                    // 0b00000100
```

## See Also

### Bitwise Operations

static func &amp; (Int, Int) -> Int

Returns the result of performing a bitwise AND operation on the two given values.

static func ~ (Self) -> Self

Returns the inverse of the bits set in the argument.

