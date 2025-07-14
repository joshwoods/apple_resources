

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  handleFault 

Instance Method

# handleFault

macOS 10.11.4+

``` source
IOReturn handleFault(void *_pager, mach_vm_size_t sourceOffset, mach_vm_size_t length);
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

- doUnmap

- redirect

