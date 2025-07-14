

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  CreateSubMemoryDescriptor_Impl 

Type Method

# CreateSubMemoryDescriptor_Impl

macOS 11.0+

``` source
static kern_return_t CreateSubMemoryDescriptor_Impl(uint64_t memoryDescriptorCreateOptions, uint64_t offset, uint64_t length, IOMemoryDescriptor *ofDescriptor, IOMemoryDescriptor **memory);
```

