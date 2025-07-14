

- Swift
- FixedWidthInteger
-  bitWidth 

Type Property

# bitWidth

The number of bits used for the underlying binary representation of values of this type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var bitWidth: Int { get }
```

**Required** Default implementation provided.

## Discussion

An unsigned, fixed-width integer type can represent values from 0 through `(2 ** bitWidth) - 1`, where `**` is exponentiation. A signed, fixed-width integer type can represent values from `-(2 ** (bitWidth - 1))` through `(2 ** (bitWidth - 1)) - 1`. For example, the `Int8` type has a `bitWidth` value of 8 and can store any integer in the range `-128...127`.

## Default Implementations

### BinaryInteger Implementations

var bitWidth: Int

The number of bits in the current binary representation of this value.

