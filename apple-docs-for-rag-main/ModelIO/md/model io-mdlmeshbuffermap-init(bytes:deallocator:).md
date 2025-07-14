

- Model I/O
- MDLMeshBufferMap
-  init(bytes:deallocator:) 

Initializer

# init(bytes:deallocator:)

Initializes a buffer map object to manage access to the specified memory.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    bytes: UnsafeMutableRawPointer,
    deallocator: (() -> Void)? = nil
)
```

## Parameters 

`bytes`  

A pointer to the data buffer to be managed by the buffer map.

`deallocator`  

Model I/O calls this block when the buffer map object is deallocated. Use this block to unmap a shared buffer or perform other cleanup tasks.

The block has no parameters and no return value.

## Return Value

A new buffer map object.

