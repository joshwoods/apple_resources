

- Kernel
- IOKit Fundamentals
- Memory
- IODMACommand
-  MappingOptions 

# MappingOptions

Mapping types to indicate the desired mapper type for translating memory descriptors into I/O DMA Bus addresses.

``` source
enum MappingOptions {
   kMapped = 0x00000000,
   kBypassed = 0x00000001,
   kNonCoherent = 0x00000002,
   kTypeMask = 0x0000000f,
   kNoCacheStore = 0x00000010, // Memory in descriptor
   kOnChip = 0x00000020, // Indicates DMA is on South Bridge
   kIterateOnly = 0x00000040 // DMACommand will be used as a cursor only
};
```

## Topics

### Constants

kNonCoherent

kMapped

kBypassed

kMaxMappingOptions

## See Also

### Creating a DMA Command

withSpecification

Creates and initializes a DMA command in one operation.

+ withSpecification

Creates and initializes an DMA command in one operation.

+ withSpecification

Creates and initializes an DMA command in one operation.

initWithSpecification

Primary initializer for the DMA command object.

- initWithSpecification

Primary initializer for the DMA command object.

- initWithSpecification

Primary initializer for the DMA command object.

weakWithSpecification

Creates and initializes an DMA command object in one operation if this version of the operating system supports it.

+ withRefCon

- initWithRefCon

cloneCommand

Creates a new command based on the specification of the current one.

- cloneCommand

Creates a new command based on the specification of the current one.

- init

- free

SynchronizeOptions

Options for the synchronize method.

