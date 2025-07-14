

- Kernel
- Hardware Families
- FireWire
-  IOFWPseudoAddressSpace 

Class

# IOFWPseudoAddressSpace

macOS 10.0+

``` source
class IOFWPseudoAddressSpace : IOFWAddressSpace
```

## Topics

### Miscellaneous

contains

returns number of bytes starting at addr in this space

doRead

A method for processing an address space read request

doWrite

A method for processing an address space write request

initAll

Initialize an address space object to handle r/w memory

initFixed

Initialize a fixed address space at top of kCSRRegisterSpaceBaseAddressHi

setARxReqIntCompleteHandler

Installs a callback to receive notification, when FWIM has completed ARxReqInt processing and no incoming packets are left in the queue.

simpleRead

Create an address space object to handle read-only memory (eg. the local ROM) handles everything itself

simpleReader

A method for processing an address space read request

simpleReadFixed

Create an address space object to handle fixed read-only memory (eg. the local ROM) handles everything itself

simpleRW(IOFireWireBus *, FWAddress *, IOMemoryDescriptor *)

Create an address space object to handle r/w memory handles everything itself

simpleRW(IOFireWireBus *, FWAddress *, UInt32, void *)

Create an address space object to handle r/w memory handles everything itself

simpleRWFixed

Create a Read/Write fixed address space at top of kCSRRegisterSpaceBaseAddressHi.

simpleWriter

A method for processing an address space write request

### DataTypes

ExpansionData

### Instance Variables

reserved

### Instance Methods

- allocateAddress

- contains

- createAuxiliary

- doRead

- doWrite

- free

- freeAddress

- getMetaClass

- handleARxReqIntComplete

- initAll

- initFixed

- setARxReqIntCompleteHandler

### Type Methods

+ readWrite

+ simpleRW

+ simpleRW

+ simpleRWFixed

+ simpleRead

+ simpleReadFixed

+ simpleReader

+ simpleWriter

## Relationships

### Inherits From

- IOFWAddressSpace

## See Also

### Address Spaces

IOFWAddressSpaceAux

IOFWPhysicalAddressSpaceAux

IOFWPseudoAddressSpaceAux

IOFWSimpleContiguousPhysicalAddressSpace

IOFireWirePCRSpace

object to multiplex users of the PCR plug registers

IOFWSimplePhysicalAddressSpace

IOFWPhysicalAddressSpace

IOFWAddressSpace

