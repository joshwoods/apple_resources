

- Foundation
- NSData
-  init(bytesNoCopy:length:freeWhenDone:) 

Initializer

# init(bytesNoCopy:length:freeWhenDone:)

Initializes a newly allocated data object by adding the given number of bytes from the given buffer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    bytesNoCopy bytes: UnsafeMutableRawPointer,
    length: Int,
    freeWhenDone b: Bool
)
```

## Parameters 

`bytes`  

A buffer containing data for the new object. If `flag` is true, `bytes` must point to a memory block allocated with `malloc`.

`length`  

The number of bytes to hold from `bytes`. This value must not exceed the length of `bytes`.

`b`  

If true, the returned object takes ownership of the `bytes` pointer and frees it on deallocation.

## See Also

### Creating Data

init(bytes: UnsafeRawPointer?, length: Int)

Initializes a data object filled with a given number of bytes copied from a given buffer.

init(bytesNoCopy: UnsafeMutableRawPointer, length: Int)

Initializes a data object filled with a given number of bytes of data from a given buffer.

init(bytesNoCopy: UnsafeMutableRawPointer, length: Int, deallocator: ((UnsafeMutableRawPointer, Int) -> Void)?)

Initializes a data object filled with a given number of bytes of data from a given buffer, with a custom deallocator block.

init(data: Data)

Initializes a data object with the contents of another data object.

