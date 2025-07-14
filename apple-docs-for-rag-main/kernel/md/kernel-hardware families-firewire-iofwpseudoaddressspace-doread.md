

- Kernel
- Hardware Families
- FireWire
- IOFWPseudoAddressSpace
-  doRead 

# doRead

A method for processing an address space read request

``` source
virtual UInt32 doRead( 
 UInt16nodeID, 
 IOFWSpeed & speed, 
 FWAddressaddr, 
 UInt32len, 
 IOMemoryDescriptor **buf, 
 IOByteCount *offset, 
 IOFWRequestRefConreqrefcon); 
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

`reqrefcon`  

Can be queried for extra info about the request.

## Return Value

UIn32 returns kFWResponseComplete on success

## See Also

### Miscellaneous

contains

returns number of bytes starting at addr in this space

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

