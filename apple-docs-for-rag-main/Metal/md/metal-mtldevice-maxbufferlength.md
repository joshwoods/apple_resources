

- Metal
- MTLDevice
-  maxBufferLength 

Instance Property

# maxBufferLength

The largest amount of memory, in bytes, that a GPU device can allocate to a buffer instance.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
var maxBufferLength: Int { get }
```

**Required**

## Discussion

The property’s value is at least 256 MB (268,435,456 bytes).

## See Also

### Creating Buffers

func makeBuffer(length: Int, options: MTLResourceOptions) -> (any MTLBuffer)?

Creates a buffer the method clears with zero values.

**Required**

func makeBuffer(bytes: UnsafeRawPointer, length: Int, options: MTLResourceOptions) -> (any MTLBuffer)?

Allocates a new buffer of a given length and initializes its contents by copying existing data into it.

**Required**

func makeBuffer(bytesNoCopy: UnsafeMutableRawPointer, length: Int, options: MTLResourceOptions, deallocator: ((UnsafeMutableRawPointer, Int) -> Void)?) -> (any MTLBuffer)?

Creates a buffer that wraps an existing contiguous memory allocation.

**Required**

