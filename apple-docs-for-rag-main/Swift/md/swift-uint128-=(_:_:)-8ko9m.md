

- Swift
- UInt128
-  \|=(\_:\_:) 

Operator

# \|=(\_:\_:)

Stores the result of performing a bitwise OR operation on the two given values in the left-hand-side variable.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func |= (a: inout UInt128, b: UInt128)
```

## Discussion

A bitwise OR operation results in a value that has each bit set to `1` where *one or both* of its arguments have that bit set to `1`. For example:

```
var x: UInt8 = 5          // 0b00000101
let y: UInt8 = 14         // 0b00001110
x |= y                    // 0b00001111
```

