

- Kernel
- Hardware Families
- FireWire
- IOFWPseudoAddressSpace
-  simpleRW(IOFireWireBus \*, FWAddress \*, IOMemoryDescriptor \*) 

# simpleRW(IOFireWireBus \*, FWAddress \*, IOMemoryDescriptor \*)

Create an address space object to handle r/w memory handles everything itself

``` source
static IOFWPseudoAddressSpace* simpleRW( 
 IOFireWireBus *bus, 
 FWAddress *addr, 
 IOMemoryDescriptor *data); 
```

## Parameters 

`bus`  

Points to IOFireWireBus object.

`addr`  

Points to starting address for the Pseudo Address Space.

`data`  

The virtual address of the first byte in the memory.

## Return Value

returns valid IOFWPseudoAddressSpace on success, null on failure

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

setARxReqIntCompleteHandler

Installs a callback to receive notification, when FWIM has completed ARxReqInt processing and no incoming packets are left in the queue.

simpleRead

Create an address space object to handle read-only memory (eg. the local ROM) handles everything itself

simpleReader

A method for processing an address space read request

simpleReadFixed

Create an address space object to handle fixed read-only memory (eg. the local ROM) handles everything itself

simpleRW(IOFireWireBus *, FWAddress *, UInt32, void *)

Create an address space object to handle r/w memory handles everything itself

simpleRWFixed

Create a Read/Write fixed address space at top of kCSRRegisterSpaceBaseAddressHi.

simpleWriter

A method for processing an address space write request

