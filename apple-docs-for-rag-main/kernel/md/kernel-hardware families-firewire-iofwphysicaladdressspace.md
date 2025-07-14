

- Kernel
- Hardware Families
- FireWire
-  IOFWPhysicalAddressSpace 

Class

# IOFWPhysicalAddressSpace

macOS 10.0+

``` source
class IOFWPhysicalAddressSpace : IOFWAddressSpace
```

## Topics

### Miscellaneous

checkMemoryInRange

Validates the IOMemoryDescriptor, which is used to initialize the PhysicalAddressSpace.

complete

complete the IODMACommand used by this PhysicalAddressSpace.

doRead

A method for processing an address space read request

doWrite

A method for processing an address space write request

getDMACommand

Get the DMACommand from this PhysicalAddressSpace.

getLength

Get the length of the memory backed by PhysicalAddressSpace.

getMemoryDescriptor

Gets the memory descriptor, which is associated to this PhysicalAddressSpace.

getSegments

Returns the scatter gather list of memory segments from the IODMACommand used in this PhysicalAddressSpace.

init

Initialize physical address space.

initWithDesc

Initialize physical address space with IOMemoryDescriptor.

initWithDMACommand

Initialize physical address space with IODMACommand.

isPrepared

Inspects whether the IODMACommand was prepared in this PhysicalAddressSpace.

prepare

Prepare the IODMACommand used by this PhysicalAddressSpace.

setDMACommand

Set the DMACommand for this PhysicalAddressSpace.

setMemoryDescriptor

Sets the memory descriptor, which will be associated to this PhysicalAddressSpace.

synchronize

synchronize the IODMACommand used by this PhysicalAddressSpace.

### Instance Methods

- checkMemoryInRange

- complete

- createAuxiliary

- doRead

- doWrite

- free

- getDMACommand

- getLength

- getMemoryDescriptor

- getMetaClass

- getPhysicalSegment

- getSegments

- init

- initWithDMACommand

- initWithDesc

- isPrepared

- prepare

- setDMACommand

- setMemoryDescriptor

- synchronize

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

IOFWPseudoAddressSpace

IOFWSimplePhysicalAddressSpace

IOFWAddressSpace

