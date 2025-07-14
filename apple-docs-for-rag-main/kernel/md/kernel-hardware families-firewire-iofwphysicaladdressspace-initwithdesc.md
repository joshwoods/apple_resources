

- Kernel
- Hardware Families
- FireWire
- IOFWPhysicalAddressSpace
-  initWithDesc 

# initWithDesc

Initialize physical address space with IOMemoryDescriptor.

``` source
virtual bool initWithDesc(
 IOFireWireBus *bus, 
 IOMemoryDescriptor *mem); 
```

## Parameters 

`bus`  

Points to IOFireWireBus object.

`mem`  

Points to IOMemoryDescriptor.

## Return Value

returns true if success, else false

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

getSegments

Returns the scatter gather list of memory segments from the IODMACommand used in this PhysicalAddressSpace.

init

Initialize physical address space.

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

