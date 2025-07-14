

- Kernel
- Hardware Families
- FireWire
- IOFWPseudoAddressSpace
-  setARxReqIntCompleteHandler 

# setARxReqIntCompleteHandler

Installs a callback to receive notification, when FWIM has completed ARxReqInt processing and no incoming packets are left in the queue.

``` source
inline void setARxReqIntCompleteHandler(
 void *refcon,
 IOFWARxReqIntCompleteHandlerhandler ) 
```

## Parameters 

`refcon`  

Client's callback object.

`handler`  

Client callback to be invoked, at the end of interrupt processing.

## Return Value

none.

## See Also

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

