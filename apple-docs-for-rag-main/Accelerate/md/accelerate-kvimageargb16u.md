

- Accelerate
-  kvImageARGB16U 

Global Variable

# kvImageARGB16U

Any 16-bit unsigned, four-channel interleaved buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var kvImageARGB16U: vImageARGBType { get }
```

## Discussion

This type doesn’t specify channel order.

## See Also

### Constants

init(UInt32)

Creates a new ARGB type.

init(rawValue: UInt32)

Creates a new ARGB type with an unsigned integer value.

var rawValue: UInt32

The unsigned integer raw value.

var kvImageARGB16Q12: vImageARGBType

Any 8-bit four-channel interleaved buffer.

var kvImageARGB8888: vImageARGBType

Any 16-bit signed fixed-point, four-channel interleaved buffer.

