

- Kernel
- IOKit Fundamentals
- 
  - IOKit Fundamentals
- Memory
- IODMACommand
- Private Accessors
-  PerformOperation 

Instance Method

# PerformOperation

macOS 11.0+

``` source
kern_return_t PerformOperation(uint64_t options, uint64_t dmaOffset, uint64_t length, uint64_t dataOffset, IOMemoryDescriptor *data, OSDispatchMethod supermethod);
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

- GetPreparation

- GetPreparation_Impl

- PerformOperation

- PerformOperation_Impl

- PrepareForDMA

- PrepareForDMA

- PrepareForDMA_Impl

