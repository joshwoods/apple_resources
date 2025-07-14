

- Kernel
- IOKit Fundamentals
- 
  - IOKit Fundamentals
- Memory
- IODMACommand
- Private Accessors
-  PrepareForDMA_Invoke 

Type Method

# PrepareForDMA_Invoke

macOS 11.0+

``` source
static kern_return_t PrepareForDMA_Invoke(const IORPC rpc, OSMetaClassBase *target, PrepareForDMA_Handler func);
```

## See Also

### Callbacks

+ CompleteDMA_Invoke

+ Create

+ Create_Impl

+ Create_Invoke

+ GetPreparation_Invoke

+ PerformOperation_Invoke

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

