

- Kernel
- IOKit Fundamentals
- Memory
- IODMACommand
-  weakWithSpecification 

# weakWithSpecification

Creates and initializes an DMA command object in one operation if this version of the operating system supports it.

``` source
static inline IOReturn weakWithSpecification (
 IODMACommand **newCommand, 
 SegmentFunction outSegFunc, 
 UInt8 numAddressBits, 
 UInt64 maxSegmentSize, 
 MappingOptions mapType = kMapped, 
 UInt64 maxTransferSize = 0, 
 UInt32 alignment = 1, 
 IOMapper *mapper = 0, 
 void *refCon = 0) __attribute__((always_inline)); 
```

## Parameters 

`newCommand`  

Output reference variable of the newly created IODMACommand.

`outSegFunc`  

SegmentFunction to call to output one physical segment. A set of nine commonly required segment functions are provided.

`numAddressBits`  

Number of bits that the hardware uses on its internal address bus. Typically 32 but may be more on modern hardware. A 0 implies no-restriction other than that implied by the output segment function.

`maxSegmentSize`  

Maximum allowable size for one segment. Zero is treated as an unlimited segment size.

`mapType`  

is the type of mapping that is required to translate an IOMemoryDescriptor into the desired number of bits. For instance if your hardware only supports 32 bits but must run on machines with \> 4G of RAM some mapping will be required. Number of bits will be specified in numAddressBits, see below. This parameter can take 3 values:- kNonCoherent - used for non-coherent hardware transfers, Mapped - Validate that all I/O bus generated addresses are within the number of addressing bits specified, Bypassed indicates that bypassed addressing is required, this is used when the hardware transfers are into coherent memory but no mapping is required. See also prepare() for failure cases.

`maxTransferSize`  

Maximum size of an entire transfer. Defaults to 0 indicating no maximum.

`alignment`  

Alignment restriction, in bytes, on I/O bus addresses. Defaults to single byte alignment.

`mapper`  

For mapping types kMapped & kBypassed mapper is used to define the hardware that will perform the mapping, defaults to the system mapper.

## Return Value

kIOReturnSuccess if everything is OK, otherwise kIOReturnBadArgument if newCommand is NULL, kIOReturnUnsupported if the kernel doesn't export IODMACommand or IOReturnError if the new command fails to init, q.v. initWithSpecification.

## Overview

Factory function to create and initialise an IODMACommand in one operation. The function allows a developer to 'weak' link with IODMACommand. This function will return kIOReturnUnsupported if the IODMACommand is unavailable. This function is actually fairly slow so it will be better to call it once then clone the successfully create command using cloneCommand (q.v.).

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

