

- Kernel
- Hardware Families
- FireWire
- IOFWAddressSpace
-  doRead 

# doRead

An abstract method for processing an address space read request

``` source
virtual UInt32 doRead(
 UInt16nodeID,
 IOFWSpeed &speed,
 FWAddressaddr,
 UInt32len, 
 IOMemoryDescriptor **buf,
 IOByteCount *offset, 
 IOFWRequestRefConrefcon) = 0; 
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

activate

Address space is ready for handling requests.

addTrustedNode

Add a trusted node.

contains

returns number of bytes starting at addr in this space

deactivate

Address space request handler is disabled.

doLock

A method for processing a lock request.

doWrite

An abstract method for processing an address space write request

intersects

Checks this address space intersects with the given address range. Currently only supports IOFWPsuedoAddressSpaces.

isExclusive

Checks if an address space wants exclusive control of its address range

isTrustedNode

returns true if the node is added as a trusted node

removeAllTrustedNodes

Remove all trusted nodes.

removeTrustedNode

Remove a trusted node.

setExclusive

Sets if this address space requires exclusive control of its address range. Exclusivity should be set before an address space is activated.

