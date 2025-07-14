

- Kernel
- IOKit Fundamentals
- Memory
- IODMACommand
-  withSpecification 

Type Method

# withSpecification

Creates and initializes an DMA command in one operation.

macOS 10.15.2+

``` source
static OSPtr withSpecification(SegmentFunction outSegFunc, const SegmentOptions *segmentOptions, uint32_t mappingOptions, IOMapper *mapper, void *refCon);
```

## Parameters 

`outSegFunc`  

SegmentFunction to call to output one physical segment. A set of nine commonly required segment functions are provided.

`segmentOptions`  

A structure with the segment configuration options.

`mappingOptions`  

The type of mapping that is required to translate an IOMemoryDescriptor into the desired number of bits. For instance if your hardware only supports 32 bits but must run on machines with \> 4G of RAM some mapping will be required. Number of bits will be specified in numAddressBits, see below.This parameter can take 3 values:- kNonCoherent - used for non-coherent hardware transfers, Mapped - Validate that all I/O bus generated addresses are within the number of addressing bits specified, Bypassed indicates that bypassed addressing is required, this is used when the hardware transferes are into coherent memory but no mapping is required. See also prepare() for failure cases.

`mapper`  

For mapping types kMapped & kBypassed mapper is used to define the hardware that will perform the mapping, defaults to the system mapper.

`refCon`  

A reference constant for the object.

## Return Value

Returns a new memory cursor if successfully created and initialized, 0 otherwise.

## Discussion

Factory function to create and initialize an IODMACommand in one operation.

## See Also

### Creating a DMA Command

withSpecification

Creates and initializes a DMA command in one operation.

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

MappingOptions

Mapping types to indicate the desired mapper type for translating memory descriptors into I/O DMA Bus addresses.

SynchronizeOptions

Options for the synchronize method.

