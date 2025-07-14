

- Kernel
- IOKit Fundamentals
- Memory
- IOSubMemoryDescriptor
-  makeMapping 

Instance Method

# makeMapping

macOS 10.11.4+

``` source
virtual IOMemoryMap * makeMapping(IOMemoryDescriptor *owner, task_t intoTask, IOVirtualAddress atAddress, IOOptionBits options, IOByteCount offset, IOByteCount length);
```

