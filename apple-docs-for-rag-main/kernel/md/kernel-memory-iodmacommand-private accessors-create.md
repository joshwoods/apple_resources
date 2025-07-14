

- Kernel
- IOKit Fundamentals
- 
  - IOKit Fundamentals
- Memory
- IODMACommand
- Private Accessors
-  Create 

Type Method

# Create

DriverKitKernelDriverKit 20.0+macOS 11.0+

``` source
static kern_return_t Create(IOService *device, uint64_t options, const IODMACommandSpecification *specification, IODMACommand **command);
```

## See Also

### Callbacks

+ CompleteDMA_Invoke

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

