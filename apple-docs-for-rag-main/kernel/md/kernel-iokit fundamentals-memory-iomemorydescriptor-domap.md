

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  doMap 

Instance Method

# doMap

macOS 10.11.4+

``` source
virtual IOReturn doMap(vm_map_t addressMap, IOVirtualAddress *atAddress, IOOptionBits options, IOByteCount sourceOffset, IOByteCount length);
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

- doUnmap

- handleFault

- redirect

