

- Kernel
- Hardware Families
- FireWire
-  IOFireWireBus 

Class

# IOFireWireBus

IOFireWireBus is a public class the provides access to general FireWire functionality...

macOS 10.0+

``` source
class IOFireWireBus : IOService
```

## Overview

## Topics

### Miscellaneous

createLocalIsochPort

Create a local isochronous port to run the given DCL program

### Instance Methods

- AddUnitDirectory

- RemoveUnitDirectory

- createAsyncStreamCommand

- createAsyncStreamCommand

- createAuxiliary

- createDCLPool

- createDelayedCmd

- createInitialAddressSpace

- createIsochChannel

- createLocalIsochPort

- createPhysicalAddressSpace

- createPseudoAddressSpace

- createSimpleContiguousPhysicalAddressSpace

- createSimplePhysicalAddressSpace

- getAddressSpace

- getBusCycleTime

- getBusPowerManager

- getCycleTime

- getExtendedTCode

- getFireWirePhysicalAddressBits

- getFireWirePhysicalAddressMask

- getFireWirePhysicalBufferBits

- getFireWirePhysicalBufferMask

- getMaxRec

- getMetaClass

- getSessionRefExporter

- hopCount

- hopCount

- isCompleteRequest

- isLockRequest

- isQuadRequest

- makeRoot

- maxPackLog

- maxPackLog

- nodeIDtoDevice

- resetBus

## Relationships

### Inherits From

- IOService

## See Also

### Interfaces

IOFireWireSerialBusProtocolTransport

SCSI Protocol Driver Family for FireWire SBP2 Devices.

IOFireWireSBP2Target

Serves as bridge between IOFireWireUnit and IOFireWireLUN.

IOFireWireController

