

- Kernel
- Hardware Families
- FireWire
-  IOFireWireNub 

Class

# IOFireWireNub

macOS 10.0+

``` source
class IOFireWireNub : IOService
```

## Topics

### Instance Methods

- FWSpeed

- FWSpeed

- clearNodeFlags

- createAuxiliary

- createCompareAndSwapCommand

- createPhysicalAddressSpace

- createPseudoAddressSpace

- createReadCommand

- createReadQuadCommand

- createSimpleContiguousPhysicalAddressSpace

- createSimplePhysicalAddressSpace

- createWriteCommand

- createWriteQuadCommand

- free

- getBus

- getConfigDirectory

- getConfigDirectoryRef

- getController

- getMetaClass

- getNodeFlags

- getNodeIDGeneration

- getNodeIDGeneration

- getTerminationState

- getUniqueID

- hopCount

- hopCount

- init

- isPhysicalAccessEnabled

- maxPackLog

- maxPackLog

- maxPackLog

- setConfigDirectory

- setMaxPackLog

- setNodeFlags

- setTerminationState

## Relationships

### Inherits From

- IOService

## See Also

### Nubs

IOFireWireLocalNode

IOFireWireSBP2LUN

Provider for most drivers.

IOFireWireAVCSubUnit

nub for sub unit of AVC devices. Just for matching, calls the AVC unit for all functions.

IOFireWireAVCUnit

nub for AVC devices

IOFireWireAVCNub

nub for AVC devices

IOFireWireUnit

