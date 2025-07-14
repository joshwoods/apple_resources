

- Kernel
- IOKit Fundamentals
- Memory
- IOMapper
-  iovmMapMemory 

Instance Method

# iovmMapMemory

macOS 10.11.4+

``` source
virtual IOReturn iovmMapMemory(IOMemoryDescriptor *memory, uint64_t descriptorOffset, uint64_t length, uint32_t mapOptions, const IODMAMapSpecification *mapSpecification, IODMACommand *dmaCommand, const IODMAMapPageList *pageList, uint64_t *mapAddress, uint64_t *mapLength);
```

## See Also

### Mapping Memory Addresses

- mapToPhysicalAddress

- iovmUnmapMemory

- iovmInsert

