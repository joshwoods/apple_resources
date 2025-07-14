

- Kernel
- Hardware Families
- FireWire
- IOFWAddressSpace
-  doLock 

# doLock

A method for processing a lock request.

``` source
virtual UInt32 doLock(
 UInt16nodeID,
 IOFWSpeed &speed,
 FWAddressaddr,
 UInt32inlen, 
 const UInt32 *newVal,
 UInt32 &outLen,
 UInt32 *oldVal, 
 UInt32extType,
 IOFWRequestRefConrefcon); 
```

## Parameters 

`nodeID`  

FireWire Lock request for nodeID.

`speed`  

at this 'speed'.

`addr`  

with FireWire address 'addr'.

`inlen`  

'inlen' bytes to use.

`newVal`  

new value to write at 'addr' location .

`outLen`  

'outLen' bytes for result.

`oldVal`  

old value read from 'addr' location.

`extType`  

Type like kFWExtendedTCodeCompareSwap.

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

doRead

An abstract method for processing an address space read request

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

