

- Kernel
- IOKit Fundamentals
- 
  - IOKit Fundamentals
- Memory
- IODMACommand
- Private Accessors
-  GetPreparation 

Instance Method

# GetPreparation

macOS 11.0+

``` source
kern_return_t GetPreparation(uint64_t *offset, uint64_t *length, IOMemoryDescriptor **memory, OSDispatchMethod supermethod);
```

## See Also

### Callbacks

+ CompleteDMA_Invoke

+ Create

+ Create_Impl

+ Create_Invoke

+ GetPreparation_Invoke

+ PerformOperation_Invoke

+ PrepareForDMA_Invoke

- CompleteDMA

- CompleteDMA

- CompleteDMA_Impl

- GetPreparation

- GetPreparation_Impl

- PerformOperation

- PerformOperation

- PerformOperation_Impl

- PrepareForDMA

- PrepareForDMA

- PrepareForDMA_Impl

