

- Swift
- Int
-  trailingZeroBitCount 

Instance Property

# trailingZeroBitCount

The number of trailing zeros in this value’s binary representation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var trailingZeroBitCount: Int { get }
```

## Discussion

For example, in a fixed-width integer type with a `bitWidth` value of 8, the number -8 has three trailing zeros.

```
let x = Int8(bitPattern: 0b1111_1000)
// x == -8
// x.trailingZeroBitCount == 3
```

If the value is zero, then `trailingZeroBitCount` is equal to `bitWidth`.

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

var words: Int.Words

A collection containing the words of this value’s binary representation, in order from the least significant to most significant.

struct Words

A type that represents the words of this integer.

