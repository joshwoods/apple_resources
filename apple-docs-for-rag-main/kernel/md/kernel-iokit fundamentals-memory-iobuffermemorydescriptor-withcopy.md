

- Kernel
- IOKit Fundamentals
- Memory
- IOBufferMemoryDescriptor
-  withCopy 

Type Method

# withCopy

Creates a memory buffer with memory descriptor for that buffer.

macOS 10.15+

``` source
static OSPtr withCopy(task_t inTask, IOOptionBits options, vm_map_t sourceMap, mach_vm_address_t source, mach_vm_size_t size);
```

## Parameters 

`inTask`  

The task the buffer will be allocated in.

`options`  

Options for the allocation:

kIODirectionOut, kIODirectionIn - set the direction of the I/O transfer.

kIOMemoryPhysicallyContiguous - pass to request memory be physically contiguous. This option is heavily discouraged. The request may fail if memory is fragmented, may cause large amounts of paging activity, and may take a very long time to execute.

kIOMemoryPageable - pass to request memory be non-wired - the default for kernel allocated memory is wired.

kIOMemoryPurgeable - pass to request memory that may later have its purgeable state set with IOMemoryDescriptor::setPurgeable. Only supported for kIOMemoryPageable allocations.

kIOMemoryKernelUserShared - pass to request memory that will be mapped into both the kernel and client applications.

kIOMapInhibitCache - allocate memory with inhibited cache setting.

kIOMapWriteThruCache - allocate memory with writethru cache setting.

kIOMapCopybackCache - allocate memory with copyback cache setting.

kIOMapWriteCombineCache - allocate memory with writecombined cache setting.

`sourceMap`  

The memory map to copy from.

`source`  

The address at which to start copying.

`size`  

The number of bytes to copy.

## Return Value

Returns an instance of class IOBufferMemoryDescriptor to be released by the caller, which will free the memory desriptor and associated buffer.

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

+ withBytes

Creates a buffer memory descriptor and fills it with the specified bytes.

+ withCapacity

Creates a buffer memory descriptor and allocates enough bytes to meet the specified capacity.

- free

Performs any final cleanup for the memory buffer descriptor object.

