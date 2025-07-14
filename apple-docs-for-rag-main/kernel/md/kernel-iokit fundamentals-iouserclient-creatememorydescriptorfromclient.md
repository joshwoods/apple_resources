

- Kernel
- IOKit Fundamentals
- IOUserClient
-  CreateMemoryDescriptorFromClient 

Instance Method

# CreateMemoryDescriptorFromClient

macOS 11.0+

``` source
kern_return_t CreateMemoryDescriptorFromClient(uint64_t memoryDescriptorCreateOptions, uint32_t segmentsCount, const IOAddressSegment *segments, IOMemoryDescriptor **memory, OSDispatchMethod supermethod);
```

