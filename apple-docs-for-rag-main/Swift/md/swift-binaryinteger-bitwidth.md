

- Swift
- BinaryInteger
-  bitWidth 

Instance Property

# bitWidth

The number of bits in the current binary representation of this value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var bitWidth: Int { get }
```

**Required** Default implementation provided.

## Discussion

This property is a constant for instances of fixed-width integer types.

## Default Implementations

### BinaryInteger Implementations

var bitWidth: Int

The number of bits in the current binary representation of this value.

## See Also

### Working with Binary Representation

var trailingZeroBitCount: Int

The number of trailing zeros in this value’s binary representation.

**Required**

var words: Self.Words

A collection containing the words of this value’s binary representation, in order from the least significant to most significant.

**Required**

associatedtype Words : RandomAccessCollection

A type that represents the words of a binary integer.

**Required**

