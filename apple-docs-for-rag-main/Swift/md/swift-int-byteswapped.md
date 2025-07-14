

- Swift
- Int
-  byteSwapped 

Instance Property

# byteSwapped

A representation of this integer with the byte order swapped.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var byteSwapped: Int { get }
```

## See Also

### Working with Byte Order

var littleEndian: Self

The little-endian representation of this integer.

var bigEndian: Self

The big-endian representation of this integer.

init(littleEndian: Self)

Creates an integer from its little-endian representation, changing the byte order if necessary.

init(bigEndian: Self)

Creates an integer from its big-endian representation, changing the byte order if necessary.

