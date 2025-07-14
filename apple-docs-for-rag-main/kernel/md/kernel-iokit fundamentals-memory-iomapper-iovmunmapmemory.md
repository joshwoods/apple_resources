

- Kernel
- IOKit Fundamentals
- Memory
- IOMapper
-  iovmUnmapMemory 

Instance Method

# iovmUnmapMemory

macOS 10.11.4+

``` source
virtual IOReturn iovmUnmapMemory(IOMemoryDescriptor *memory, IODMACommand *dmaCommand, uint64_t mapAddress, uint64_t mapLength);
```

## See Also

### Mapping Memory Addresses

- mapToPhysicalAddress

- iovmMapMemory

- iovmInsert

