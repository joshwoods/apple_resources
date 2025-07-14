

- Paravirtualized Graphics
- PGPhysicalMemoryRange_s
-  init(physicalAddress:physicalLength:) 

Initializer

# init(physicalAddress:physicalLength:)

Creates a memory range.

Mac Catalyst 14.0+macOS 11.0+

``` source
init(
    physicalAddress: UInt64,
    physicalLength: UInt64
)
```

## Parameters 

`physicalAddress`  

The starting address of the range in physical memory.

`physicalLength`  

The length of the range.

## See Also

### Creating a Memory Range

init()

Creates a default memory range.

