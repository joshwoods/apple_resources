

- Kernel
- IOKit Fundamentals
- 
  - IOKit Fundamentals
- Memory
- IODMACommand
- Private Accessors
-  CompleteDMA_Invoke 

Type Method

# CompleteDMA_Invoke

macOS 11.0+

``` source
static kern_return_t CompleteDMA_Invoke(const IORPC rpc, OSMetaClassBase *target, CompleteDMA_Handler func);
```

## See Also

### Callbacks

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

- PerformOperation_Impl

- PrepareForDMA

- PrepareForDMA

- PrepareForDMA_Impl

