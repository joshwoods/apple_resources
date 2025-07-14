

- Kernel
- Hardware Families
- FireWire
-  IOFireWirePCRSpace 

Class

# IOFireWirePCRSpace

object to multiplex users of the PCR plug registers

macOS 10.2+

``` source
class IOFireWirePCRSpace : IOFWPseudoAddressSpace
```

## Overview

## Topics

### Miscellaneous

allocateInputPlug

allocates an input plug.

allocateOutputPlug

allocates an output plug.

clearAllP2PConnections

freeInputPlug

deallocates an input plug.

freeOutputPlug

deallocates an output plug.

getPCRAddressSpace

returns the IOFireWirePCRSpace object for the given FireWire bus

init

initializes the IOFireWirePCRSpace object

readInputMasterPlug

Returns the current value of the primary input plug.

readInputPlug

returns the current value of an input plug.

readOutputMasterPlug

Returns the current value of the primary output plug.

readOutputPlug

returns the current value of an output plug.

setAVCTargetSpacePointer

updateInputMasterPlug

Updates the value of the primary input plug (simulating a lock transaction).

updateInputPlug

updates the value of an input plug (simulating a lock transaction).

updateOutputMasterPlug

Updates the value of the primary output plug (simulating a lock transaction).

updateOutputPlug

updates the value of an output plug (simulating a lock transaction).

### DataTypes

ExpansionData

### Instance Variables

reserved

### Instance Methods

- activate

- allocateInputPlug

- allocateOutputPlug

- allocatePlug

- clearAllP2PConnections

- deactivate

- doWrite

- freeInputPlug

- freeOutputPlug

- freePlug

- getMetaClass

- init

- readInputMasterPlug

- readInputPlug

- readOutputMasterPlug

- readOutputPlug

- readPlug

- setAVCTargetSpacePointer

- updateInputMasterPlug

- updateInputPlug

- updateOutputMasterPlug

- updateOutputPlug

- updatePlug

### Type Methods

+ getPCRAddressSpace

## Relationships

### Inherits From

- IOFWPseudoAddressSpace

## See Also

### Address Spaces

IOFWAddressSpaceAux

IOFWPhysicalAddressSpaceAux

IOFWPseudoAddressSpaceAux

IOFWSimpleContiguousPhysicalAddressSpace

IOFWPseudoAddressSpace

IOFWSimplePhysicalAddressSpace

IOFWPhysicalAddressSpace

IOFWAddressSpace

