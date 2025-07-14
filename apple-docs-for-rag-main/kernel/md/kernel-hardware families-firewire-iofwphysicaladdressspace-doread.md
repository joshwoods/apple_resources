

- Kernel
- Hardware Families
- FireWire
- IOFWPhysicalAddressSpace
-  doRead 

# doRead

A method for processing an address space read request

``` source
virtual UInt32 doRead(
 UInt16nodeID,
 IOFWSpeed &speed,
 FWAddressaddr,
 UInt32len, 
 IOMemoryDescriptor **buf,
 IOByteCount *offset, 
 IOFWRequestRefConrefcon); 
```

## Parameters 

`nodeID`  

FireWire Read from nodeID.

`speed`  

at this 'speed'.

`addr`  

with FireWire address 'addr'.

`len`  

read 'len' bytes from nodeID.

`buf`  

points to a memory descriptor containing the packet data.

`offset`  

start from this 'offset' in 'buf'.

`refcon`  

Can be queried for extra info about the request.

## Return Value

UIn32 returns kFWResponseComplete on success

## See Also

### Miscellaneous

checkMemoryInRange

Validates the IOMemoryDescriptor, which is used to initialize the PhysicalAddressSpace.

complete

complete the IODMACommand used by this PhysicalAddressSpace.

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

