

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  populateDevicePager 

Instance Method

# populateDevicePager

macOS 10.11.4+

``` source
IOReturn populateDevicePager(void *pager, vm_map_t addressMap, mach_vm_address_t address, mach_vm_size_t sourceOffset, mach_vm_size_t length, IOOptionBits options);
```

## See Also

### Managing Internal Structures

reserved

+ initialize

- Dispatch

+ CreateMapping_Invoke

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

