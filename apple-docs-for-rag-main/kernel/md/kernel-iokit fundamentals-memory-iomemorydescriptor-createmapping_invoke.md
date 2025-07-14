

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  CreateMapping_Invoke 

Type Method

# CreateMapping_Invoke

macOS 10.15+

``` source
static kern_return_t CreateMapping_Invoke(const IORPC rpc, OSMetaClassBase *target, CreateMapping_Handler func);
```

## See Also

### Managing Internal Structures

reserved

+ initialize

- Dispatch

- populateDevicePager

- CreateMapping

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

