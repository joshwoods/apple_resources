

- Core Media
-  CMBufferQueueCreateWithHandlers(\_:\_:\_:\_:) 

Function

# CMBufferQueueCreateWithHandlers(\_:\_:\_:\_:)

Creates a buffer queue with handlers to inspect buffers.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.1+macOS 10.14.4+tvOS 12.2+visionOS 1.0+watchOS 6.0+

``` source
func CMBufferQueueCreateWithHandlers(
    _ allocator: CFAllocator?,
    _ capacity: CMItemCount,
    _ handlers: OpaquePointer,
    _ queueOut: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Creating a Queue

func CMBufferQueueCreate(allocator: CFAllocator?, capacity: CMItemCount, callbacks: UnsafePointer&lt;CMBufferCallbacks>, queueOut: UnsafeMutablePointer&lt;CMBufferQueue?>) -> OSStatus

Creates a buffer queue with callbacks to inspect buffers.

struct CMBufferCallbacks

A structure that stores the callbacks that perform buffer operations.

