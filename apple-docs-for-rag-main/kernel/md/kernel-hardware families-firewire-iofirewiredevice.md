

- Kernel
- Hardware Families
- FireWire
-  IOFireWireDevice 

Class

# IOFireWireDevice

Represents a FireWire device.

macOS 10.0+

``` source
class IOFireWireDevice : IOFireWireNub
```

## Overview

The FireWire family tries to read the configuration ROM of each device on the FireWire bus. For each device that responds with its bus information block, the FireWire family publishes an `IOFireWireDevice` object in the I/O Registry. An `IOFireWireDevice` object keeps track of the device's node ID, copies config ROM properties into the object's property list, and scans the config ROM for unit directories, publishing an `IOFireWireUnit` object for each unit directory it finds.

## Topics

### Miscellaneous

clearNodeFlags

Resets the node's characteristics.

createPhysicalAddressSpace

Creates local physical FireWire address spaces for the device to access.

createPseudoAddressSpace

Creates local pseudo FireWire address spaces for the device to access.

getNodeFlags

Retrieves the node's characteristics.

getUnitCount

Returns number of units attached to this device.

init

Initializes the nub.

setMaxSpeed

Sets the maximum speed for this node.

setNodeFlags

Sets the node's characteristics.

### DataTypes

ExpansionData

### Instance Variables

reserved

### Instance Methods

- attach

- cacheROM

- clearNodeFlags

- configureNode

- configurePhysicalFilter

- createAuxiliary

- createPhysicalAddressSpace

- createPseudoAddressSpace

- finalize

- free

- getMetaClass

- getNodeFlags

- getOpenUnitSet

- getROMBase

- getResumeTime

- getUnitCount

- handleClose

- handleIsOpen

- handleOpen

- init

- isTerminated

- latchResumeTime

- matchPropertyTable

- message

- preprocessDirectories

- processROM

- processRootDirectory

- processUnitDirectories

- readRootDirectory

- readUnitDirectories

- setMaxSpeed

- setNodeFlags

- setNodeROM

- setRegistrationState

- setUnitCount

### Type Methods

+ readROMDirGlue

+ readROMThreadFunc

+ terminateDevice

## Relationships

### Inherits From

- IOFireWireNub

