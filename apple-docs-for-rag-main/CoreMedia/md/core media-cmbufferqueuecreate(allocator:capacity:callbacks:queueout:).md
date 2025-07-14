

- Core Media
-  CMBufferQueueCreate(allocator:capacity:callbacks:queueOut:) 

Function

# CMBufferQueueCreate(allocator:capacity:callbacks:queueOut:)

Creates a buffer queue with callbacks to inspect buffers.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBufferQueueCreate(
    allocator: CFAllocator?,
    capacity: CMItemCount,
    callbacks: UnsafePointer,
    queueOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

The allocator to use for allocating the `CMBufferQueue` object. Pass `kCFAllocatorDefault` to use the default allocator.

`capacity`  

Maximum number of buffers in the queue. Pass 0 to create a queue that will grow as needed.

`callbacks`  

Callbacks the queue should use to interrogate the buffer objects. This struct is copied internally, so the client can pass a pointer to a temporary struct on the stack.

`queueOut`  

On Output, the newly created `CMBufferQueue`.

## Return Value

A result code.

## Discussion

On return, the caller owns the returned `CMBufferQueue`, and must release it when done with it.

## See Also

### Creating a Queue

func CMBufferQueueCreateWithHandlers(CFAllocator?, CMItemCount, OpaquePointer, UnsafeMutablePointer&lt;CMBufferQueue?>) -> OSStatus

Creates a buffer queue with handlers to inspect buffers.

struct CMBufferCallbacks

A structure that stores the callbacks that perform buffer operations.

