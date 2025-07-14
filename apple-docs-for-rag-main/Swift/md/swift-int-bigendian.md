

- Swift
- Int
-  bigEndian 

Instance Property

# bigEndian

The big-endian representation of this integer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var bigEndian: Self { get }
```

## Discussion

If necessary, the byte order of this value is reversed from the typical byte order of this integer type. On a big-endian platform, for any integer `x`, `x == x.bigEndian`.

## See Also

### Working with Byte Order

var byteSwapped: Int

A representation of this integer with the byte order swapped.

var littleEndian: Self

The little-endian representation of this integer.

init(littleEndian: Self)

Creates an integer from its little-endian representation, changing the byte order if necessary.

init(bigEndian: Self)

Creates an integer from its big-endian representation, changing the byte order if necessary.

