

- Kernel
- IOKit Fundamentals
- Memory
- IOBufferMemoryDescriptor
-  withBytes 

Type Method

# withBytes

Creates a buffer memory descriptor and fills it with the specified bytes.

macOS 10.11.4+

``` source
static OSPtr withBytes(const void *bytes, vm_size_t withLength, IODirection withDirection, bool withContiguousMemory);
```

## Parameters 

`bytes`  

The bytes to copy into the newly allocated buffer.

`withLength`  

The number of bytes in the `bytes` parameter.

`withDirection`  

The direction of the I/O transfer. For example: kIODirectionOut, kIODirectionIn.

`withContiguousMemory`  

A Boolean value that indicates whether to use a contiguous block of memory for the descriptor’s buffer.

## See Also

### Creating a Memory Buffer Descriptor

inTaskWithOptions

Creates a memory buffer with memory descriptor for that buffer.

+ inTaskWithOptions

Creates a memory buffer with memory descriptor for that buffer.

+ inTaskWithOptions

Creates a memory buffer with memory descriptor for that buffer.

inTaskWithPhysicalMask

Creates a memory buffer with memory descriptor for that buffer.

+ inTaskWithPhysicalMask

Creates a memory buffer with memory descriptor for that buffer.

- initWithPhysicalMask

Creates a memory buffer with memory descriptor for that buffer.

+ withOptions

Creates a memory buffer with memory descriptor for that buffer.

+ withCapacity

Creates a buffer memory descriptor and allocates enough bytes to meet the specified capacity.

+ withCopy

Creates a memory buffer with memory descriptor for that buffer.

- free

Performs any final cleanup for the memory buffer descriptor object.

