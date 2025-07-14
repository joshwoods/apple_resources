

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  redirect 

Instance Method

# redirect

macOS 10.11.4+

``` source
virtual IOReturn redirect(task_t safeTask, bool redirect);
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

- handleFault

