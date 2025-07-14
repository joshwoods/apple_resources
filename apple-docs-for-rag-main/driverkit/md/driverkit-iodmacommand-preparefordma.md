

- DriverKit
- IODMACommand
-  PrepareForDMA 

Instance Method

# PrepareForDMA

DriverKitiOSiPadOSmacOS

``` source
kern_return_t PrepareForDMA(uint64_t options, IOMemoryDescriptor * memory, uint64_t offset, uint64_t length, uint64_t * flags, uint32_t * segmentsCount, IOAddressSegment segments[32]);
```

## See Also

### Performing Internal Operations

CompleteDMA

GetPreparation

PerformOperation

