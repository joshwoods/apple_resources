

- Foundation
- NSData
-  init(bytesNoCopy:length:) 

Initializer

# init(bytesNoCopy:length:)

Initializes a data object filled with a given number of bytes of data from a given buffer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    bytesNoCopy bytes: UnsafeMutableRawPointer,
    length: Int
)
```

## Parameters 

`bytes`  

A buffer containing data for the new object. `bytes` must point to a memory block allocated with `malloc`.

`length`  

The number of bytes to hold from `bytes`. This value must not exceed the length of `bytes`.

## Return Value

A data object initialized by adding to it `length` bytes of data from the buffer `bytes`. The returned object might be different than the original receiver.

## Discussion

The returned object takes ownership of the `bytes` pointer and frees it on deallocation. Therefore, `bytes` must point to a memory block allocated with `malloc`.

## See Also

### Creating Data

init(bytes: UnsafeRawPointer?, length: Int)

Initializes a data object filled with a given number of bytes copied from a given buffer.

init(bytesNoCopy: UnsafeMutableRawPointer, length: Int, deallocator: ((UnsafeMutableRawPointer, Int) -> Void)?)

Initializes a data object filled with a given number of bytes of data from a given buffer, with a custom deallocator block.

init(bytesNoCopy: UnsafeMutableRawPointer, length: Int, freeWhenDone: Bool)

Initializes a newly allocated data object by adding the given number of bytes from the given buffer.

init(data: Data)

Initializes a data object with the contents of another data object.

