

- Kernel
- Hardware Families
- FireWire
- IOFWPhysicalAddressSpace
-  initWithDMACommand 

# initWithDMACommand

Initialize physical address space with IODMACommand.

``` source
virtual bool initWithDMACommand(
 IOFireWireBus *bus,
 IODMACommand *command ); 
```

## Parameters 

`bus`  

Points to IOFireWireBus object.

`command`  

Points to IODMACommand.

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

initWithDesc

Initialize physical address space with IOMemoryDescriptor.

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

