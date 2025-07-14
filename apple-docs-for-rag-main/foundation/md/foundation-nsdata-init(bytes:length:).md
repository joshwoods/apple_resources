

- Foundation
- NSData
-  init(bytes:length:) 

Initializer

# init(bytes:length:)

Initializes a data object filled with a given number of bytes copied from a given buffer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    bytes: UnsafeRawPointer?,
    length: Int
)
```

## Discussion

A data object initialized by adding to it `length` bytes of data copied from the buffer `bytes`. The returned object might be different than the original receiver.

## See Also

### Creating Data

init(bytesNoCopy: UnsafeMutableRawPointer, length: Int)

Initializes a data object filled with a given number of bytes of data from a given buffer.

init(bytesNoCopy: UnsafeMutableRawPointer, length: Int, deallocator: ((UnsafeMutableRawPointer, Int) -> Void)?)

Initializes a data object filled with a given number of bytes of data from a given buffer, with a custom deallocator block.

init(bytesNoCopy: UnsafeMutableRawPointer, length: Int, freeWhenDone: Bool)

Initializes a newly allocated data object by adding the given number of bytes from the given buffer.

init(data: Data)

Initializes a data object with the contents of another data object.

