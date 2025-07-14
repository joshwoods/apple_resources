

- Metal
- MTLDevice
-  makeBuffer(bytesNoCopy:length:options:deallocator:) 

Instance Method

# makeBuffer(bytesNoCopy:length:options:deallocator:)

Creates a buffer that wraps an existing contiguous memory allocation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeBuffer(
    bytesNoCopy pointer: UnsafeMutableRawPointer,
    length: Int,
    options: MTLResourceOptions = [],
    deallocator: ((UnsafeMutableRawPointer, Int) -> Void)? = nil
) -> (any MTLBuffer)?
```

**Required**

## Parameters 

`pointer`  

A page-aligned pointer to the starting memory address.

`length`  

The size of the new buffer, in bytes, that results in a page-aligned region of memory.

`options`  

An MTLResourceOptions instance that sets the buffer’s storage and hazard-tracking modes. See Resource Fundamentals and Setting Resource Storage Modes for more information.

`deallocator`  

A block the framework invokes when it deallocates the buffer so that your app can release the underlying memory; otherwise `nil` to opt out.

## Return Value

A new MTLBuffer instance if the method completes successfully; otherwise `nil`.

## Discussion

Important

The existing memory allocation must exist within a single virtual memory (VM) region.

## See Also

### Creating Buffers

var maxBufferLength: Int

The largest amount of memory, in bytes, that a GPU device can allocate to a buffer instance.

**Required**

func makeBuffer(length: Int, options: MTLResourceOptions) -> (any MTLBuffer)?

Creates a buffer the method clears with zero values.

**Required**

func makeBuffer(bytes: UnsafeRawPointer, length: Int, options: MTLResourceOptions) -> (any MTLBuffer)?

Allocates a new buffer of a given length and initializes its contents by copying existing data into it.

**Required**

