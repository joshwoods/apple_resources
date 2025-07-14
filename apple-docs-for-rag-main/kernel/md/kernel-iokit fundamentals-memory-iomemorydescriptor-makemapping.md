

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  makeMapping 

Instance Method

# makeMapping

macOS 10.11.4+

``` source
virtual IOMemoryMap * makeMapping(IOMemoryDescriptor *owner, task_t intoTask, IOVirtualAddress atAddress, IOOptionBits options, IOByteCount offset, IOByteCount length);
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

- doMap

- doUnmap

- handleFault

- redirect

