

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  doUnmap 

Instance Method

# doUnmap

macOS 10.11.4+

``` source
virtual IOReturn doUnmap(vm_map_t addressMap, IOVirtualAddress logical, IOByteCount length);
```

## See Also

### Managing Internal Structures

reserved

+ initialize

- Dispatch

+ CreateMapping_Invoke

- populateDevicePager

- CreateMapping

- CreateMapping_Impl

- Map

Maps memory internally.

- addMapping

- removeMapping

- makeMapping

- doMap

- handleFault

- redirect

