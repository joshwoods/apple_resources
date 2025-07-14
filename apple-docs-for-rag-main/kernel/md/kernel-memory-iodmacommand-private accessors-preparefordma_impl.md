

- Kernel
- IOKit Fundamentals
- 
  - IOKit Fundamentals
- Memory
- IODMACommand
- Private Accessors
-  PrepareForDMA_Impl 

Instance Method

# PrepareForDMA_Impl

macOS 11.0+

``` source
kern_return_t PrepareForDMA_Impl(uint64_t options, IOMemoryDescriptor *memory, uint64_t offset, uint64_t length, uint64_t *flags, uint32_t *segmentsCount, IOAddressSegment *segments);
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

- PerformOperation_Impl

- PrepareForDMA

- PrepareForDMA

