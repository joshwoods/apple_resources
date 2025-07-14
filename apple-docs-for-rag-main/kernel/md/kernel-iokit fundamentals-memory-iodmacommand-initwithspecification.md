

- Kernel
- IOKit Fundamentals
- Memory
- IODMACommand
-  initWithSpecification 

Instance Method

# initWithSpecification

Primary initializer for the DMA command object.

macOS 10.15.2+

``` source
virtual bool initWithSpecification(SegmentFunction outSegFunc, const SegmentOptions *segmentOptions, uint32_t mappingOptions, IOMapper *mapper, void *refCon);
```

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

MappingOptions

Mapping types to indicate the desired mapper type for translating memory descriptors into I/O DMA Bus addresses.

SynchronizeOptions

Options for the synchronize method.

