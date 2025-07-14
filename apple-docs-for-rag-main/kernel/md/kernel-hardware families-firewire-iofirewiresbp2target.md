

- Kernel
- Hardware Families
- FireWire
-  IOFireWireSBP2Target 

Class

# IOFireWireSBP2Target

Serves as bridge between IOFireWireUnit and IOFireWireLUN.

macOS 10.0+

``` source
class IOFireWireSBP2Target : IOService
```

## Overview

Matches against IOFireWireUnits supporting the SBP2 protocol. Creates IOFireWireSBP2LUN nubs for matching. Most drivers will match against an IOFireWireSBP2LUN, but matching against an IOFireWireSBP2Target is also supported. This can be useful in cases where a single driver wishes to control all LUNs on a device. Support for this technique is minimal, however, and the driver will be required to discover it's LUNs through the registry.

## Topics

### Miscellaneous

getFireWireUnit

Returns an IOFireWireUnit object.

handleClose

Overrideable method to control the open / close behaviour of an IOService.

handleIsOpen

Overrideable method to control the open / close behaviour of an IOService.

handleOpen

Overrideable method to control the open / close behaviour of an IOService.

matchPropertyTable

Implements SBP2 specific matching.

start

During an IOService instantiation, the start method is called when the IOService has been selected to run on the provider.

stop

During an IOService termination, the stop method is called in its clients before they are detached & it is destroyed.

### Instance Methods

- beginIOCriticalSection

- cancelMgmtAgentAccess

- clearMgmtAgentAccess

- clearTargetFlags

- completeMgmtAgentAccess

- configurePhysicalFilter

- createLUN

- endIOCriticalSection

- finalize

- free

- getFireWireUnit

- getMetaClass

- getTargetFlags

- handleClose

- handleIsOpen

- handleOpen

- matchPropertyTable

- message

- scanForLUNs

- setTargetFlags

- start

- stop

- synchMgmtAgentAccess

## Relationships

### Inherits From

- IOService

## See Also

### Interfaces

IOFireWireSerialBusProtocolTransport

SCSI Protocol Driver Family for FireWire SBP2 Devices.

IOFireWireController

IOFireWireBus

IOFireWireBus is a public class the provides access to general FireWire functionality...

