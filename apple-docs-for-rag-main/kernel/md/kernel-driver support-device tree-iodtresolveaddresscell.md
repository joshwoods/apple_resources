

- Kernel
- Driver Support
- Device Tree
-  IODTResolveAddressCell 

Function

# IODTResolveAddressCell

macOS 10.0+

``` source
bool IODTResolveAddressCell(IORegistryEntry *regEntry, UInt32 cellsIn[], IOPhysicalAddress *phys, IOPhysicalLength *len);
```

## See Also

### Registry Utilities

IODTCompareNubName

IODTFindMatchingEntries

IODTFindSlotName

IODTGetCellCounts

IODTInterruptControllerName

IODTMakeNVDescriptor

IODTMatchNubWithKeys

IODTResolveAddressing

IODTSetResolving

IODTGetInterruptOptions

IODTMapInterrupts

