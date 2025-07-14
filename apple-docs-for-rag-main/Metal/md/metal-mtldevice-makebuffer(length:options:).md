

- Metal
- MTLDevice
-  makeBuffer(length:options:) 

Instance Method

# makeBuffer(length:options:)

Creates a buffer the method clears with zero values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeBuffer(
    length: Int,
    options: MTLResourceOptions = []
) -> (any MTLBuffer)?
```

**Required**

## Parameters 

`length`  

The size of the new buffer, in bytes.

`options`  

An MTLResourceOptions instance that sets the buffer’s storage and hazard-tracking modes. See Resource Fundamentals and Setting Resource Storage Modes for more information.

## Return Value

A new MTLBuffer instance if the method completed successfully; otherwise `nil`.

## Mentioned in 

Setting Resource Storage Modes

Copying Data to a Private Resource

## See Also

### Creating Buffers

var maxBufferLength: Int

The largest amount of memory, in bytes, that a GPU device can allocate to a buffer instance.

**Required**

func makeBuffer(bytes: UnsafeRawPointer, length: Int, options: MTLResourceOptions) -> (any MTLBuffer)?

Allocates a new buffer of a given length and initializes its contents by copying existing data into it.

**Required**

func makeBuffer(bytesNoCopy: UnsafeMutableRawPointer, length: Int, options: MTLResourceOptions, deallocator: ((UnsafeMutableRawPointer, Int) -> Void)?) -> (any MTLBuffer)?

Creates a buffer that wraps an existing contiguous memory allocation.

**Required**

