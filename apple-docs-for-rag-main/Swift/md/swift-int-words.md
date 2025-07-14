

- Swift
- Int
-  words 

Instance Property

# words

A collection containing the words of this value’s binary representation, in order from the least significant to most significant.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var words: Int.Words { get }
```

## Discussion

Negative values are returned in two’s complement representation, regardless of the type’s underlying implementation.

## See Also

### Working with Binary Representation

static var bitWidth: Int

The number of bits used for the underlying binary representation of values of this type.

var bitWidth: Int

The number of bits in the current binary representation of this value.

var nonzeroBitCount: Int

The number of bits equal to 1 in this value’s binary representation.

var leadingZeroBitCount: Int

The number of leading zeros in this value’s binary representation.

var trailingZeroBitCount: Int

The number of trailing zeros in this value’s binary representation.

struct Words

A type that represents the words of this integer.

