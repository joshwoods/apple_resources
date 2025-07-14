

- Kernel
- Hardware Families
- FireWire
- IOFWPhysicalAddressSpace
-  doWrite 

# doWrite

A method for processing an address space write request

``` source
virtual UInt32 doWrite(
 UInt16nodeID,
 IOFWSpeed &speed,
 FWAddressaddr,
 UInt32len, 
 const void *buf,
 IOFWRequestRefConreqrefcon); 
```

## Parameters 

`nodeID`  

FireWire Write to nodeID.

`speed`  

at this 'speed'.

`addr`  

with FireWire address 'addr'.

`len`  

write 'len' bytes to nodeID.

`buf`  

obtain bytes from location given by 'buf'.

`reqrefcon`  

Can be queried for extra info about the request.

## Return Value

UIn32 returns kFWResponseComplete on success

## See Also

### Miscellaneous

checkMemoryInRange

Validates the IOMemoryDescriptor, which is used to initialize the PhysicalAddressSpace.

complete

complete the IODMACommand used by this PhysicalAddressSpace.

doRead

A method for processing an address space read request

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

