

- Swift
- BinaryInteger
-  words 

Instance Property

# words

A collection containing the words of this value’s binary representation, in order from the least significant to most significant.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var words: Self.Words { get }
```

**Required**

## Discussion

Negative values are returned in two’s complement representation, regardless of the type’s underlying implementation.

## See Also

### Working with Binary Representation

var bitWidth: Int

The number of bits in the current binary representation of this value.

**Required** Default implementation provided.

var trailingZeroBitCount: Int

The number of trailing zeros in this value’s binary representation.

**Required**

associatedtype Words : RandomAccessCollection

A type that represents the words of a binary integer.

**Required**

