

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  Dispatch 

Instance Method

# Dispatch

macOS 10.15+

``` source
virtual kern_return_t Dispatch(const IORPC rpc);
```

## See Also

### Managing Internal Structures

reserved

+ initialize

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

- doUnmap

- handleFault

- redirect

