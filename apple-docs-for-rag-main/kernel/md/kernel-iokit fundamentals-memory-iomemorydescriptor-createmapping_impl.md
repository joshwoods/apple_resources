

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  CreateMapping_Impl 

Instance Method

# CreateMapping_Impl

macOS 10.15+

``` source
kern_return_t CreateMapping_Impl(uint64_t options, uint64_t address, uint64_t offset, uint64_t length, uint64_t alignment, IOMemoryMap **map);
```

## See Also

### Managing Internal Structures

reserved

+ initialize

- Dispatch

+ CreateMapping_Invoke

- populateDevicePager

- CreateMapping

- Map

Maps memory internally.

- addMapping

- removeMapping

- makeMapping

- doMap

- doUnmap

- handleFault

- redirect

