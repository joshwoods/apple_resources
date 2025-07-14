

- Kernel
- IOKit Fundamentals
- Memory
- IOGeneralMemoryDescriptor
-  makeMapping 

Instance Method

# makeMapping

macOS 14.5+

``` source
virtual IOMemoryMap * makeMapping(IOMemoryDescriptor *owner, task_t intoTask, IOVirtualAddress atAddress, IOOptionBits options, IOByteCount offset, IOByteCount length);
```

