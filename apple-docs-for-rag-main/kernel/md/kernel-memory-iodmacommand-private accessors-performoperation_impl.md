

- Kernel
- IOKit Fundamentals
- 
  - IOKit Fundamentals
- Memory
- IODMACommand
- Private Accessors
-  PerformOperation_Impl 

Instance Method

# PerformOperation_Impl

macOS 11.0+

``` source
kern_return_t PerformOperation_Impl(uint64_t options, uint64_t dmaOffset, uint64_t length, uint64_t dataOffset, IOMemoryDescriptor *data);
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

- PerformOperation

- PrepareForDMA

- PrepareForDMA

- PrepareForDMA_Impl

