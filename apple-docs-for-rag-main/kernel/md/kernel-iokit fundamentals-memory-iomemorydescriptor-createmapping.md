

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  CreateMapping 

Instance Method

# CreateMapping

macOS 10.15+

``` source
kern_return_t CreateMapping(uint64_t options, uint64_t address, uint64_t offset, uint64_t length, uint64_t alignment, IOMemoryMap **map, OSDispatchMethod supermethod);
```

## See Also

### Managing Internal Structures

reserved

+ initialize

- Dispatch

+ CreateMapping_Invoke

- populateDevicePager

- CreateMapping_Impl

- Map

Maps memory internally.

- addMapping

- removeMapping

- makeMapping

- doMap

- doUnmap

- handleFault

- redirect

