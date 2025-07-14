

- Kernel
- Hardware Families
- FireWire
- IOFWPhysicalAddressSpace
-  getSegments 

# getSegments

Returns the scatter gather list of memory segments from the IODMACommand used in this PhysicalAddressSpace.

``` source
inline IOReturn getSegments(
 UInt64 *offset,
 FWSegment *fw_segments,
 UInt32 *num_segments ) ;
```

## Parameters 

`offset`  

input/output parameter, defines the starting and ending offset in the memory descriptor, relative to any offset passed to the prepare() method. FWSegment Points to an array of memory segments. num_segments Size of the FWSegment array.

## Return Value

returns kIOReturnSuccess on success

## See Also

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

