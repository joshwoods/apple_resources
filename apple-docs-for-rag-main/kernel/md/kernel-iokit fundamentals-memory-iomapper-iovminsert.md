

- Kernel
- IOKit Fundamentals
- Memory
- IOMapper
-  iovmInsert 

Instance Method

# iovmInsert

macOS 10.11.4+

``` source
virtual IOReturn iovmInsert(uint32_t options, uint64_t mapAddress, uint64_t offset, uint64_t physicalAddress, uint64_t length);
```

## See Also

### Mapping Memory Addresses

- mapToPhysicalAddress

- iovmMapMemory

- iovmUnmapMemory

