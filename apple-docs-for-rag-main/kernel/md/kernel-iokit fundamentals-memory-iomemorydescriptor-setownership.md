

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  setOwnership 

Instance Method

# setOwnership

Set the task that owns the descriptor’s memory.

macOS 10.15+

``` source
IOReturn setOwnership(task_t newOwner, int newLedgerTag, IOOptionBits newLedgerOptions);
```

## See Also

### Configuring the Descriptor

setPurgeable

Control the purgeable status of a memory descriptors memory.

- setPurgeable

Control the purgeable status of a memory descriptors memory.

