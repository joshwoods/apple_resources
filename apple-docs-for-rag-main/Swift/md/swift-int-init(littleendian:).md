

- Swift
- Int
-  init(littleEndian:) 

Initializer

# init(littleEndian:)

Creates an integer from its little-endian representation, changing the byte order if necessary.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(littleEndian value: Self)
```

## Parameters 

`value`  

A value to use as the little-endian representation of the new integer.

## See Also

### Working with Byte Order

var byteSwapped: Int

A representation of this integer with the byte order swapped.

var littleEndian: Self

The little-endian representation of this integer.

var bigEndian: Self

The big-endian representation of this integer.

init(bigEndian: Self)

Creates an integer from its big-endian representation, changing the byte order if necessary.

