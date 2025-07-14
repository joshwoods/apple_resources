

- Swift
- UnsafeMutableRawBufferPointer
-  allocate(byteCount:alignment:) 

Type Method

# allocate(byteCount:alignment:)

Allocates uninitialized memory with the specified size and alignment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func allocate(
    byteCount: Int,
    alignment: Int
) -> UnsafeMutableRawBufferPointer
```

## Parameters 

`byteCount`  

The number of bytes to allocate. `byteCount` must not be negative.

`alignment`  

The alignment of the new region of allocated memory, in bytes. `alignment` must be a whole power of 2.

## Return Value

A buffer pointer to a newly allocated region of memory aligned to `alignment`.

## Discussion

You are in charge of managing the allocated memory. Be sure to deallocate any memory that you manually allocate.

The allocated memory is not bound to any specific type and must be bound before performing any typed operations. If you are using the memory for a specific type, allocate memory using the `UnsafeMutablePointerBuffer.allocate(capacity:)` static method instead.

