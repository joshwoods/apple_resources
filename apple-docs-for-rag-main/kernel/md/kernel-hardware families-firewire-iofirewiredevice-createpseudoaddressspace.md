

- Kernel
- Hardware Families
- FireWire
- IOFireWireDevice
-  createPseudoAddressSpace 

# createPseudoAddressSpace

Creates local pseudo FireWire address spaces for the device to access.

``` source
virtual IOFWPseudoAddressSpace *createPseudoAddressSpace(
 FWAddress *addr,
 UInt32len, 
 FWReadCallbackreader,
 FWWriteCallbackwriter,
 void *refcon); 
```

## Parameters 

`addr`  

The FireWire address that is mapped to the pseudo address access.

`len`  

Size of the address space to allocate.

`reader`  

Read callback, when the device reads from this address space.

`writer`  

Write callback, when the device writes to this address space.

`refcon`  

Client's callback object returned during reader/writer callbacks.

## Return Value

A valid `IOFWPseudoAddressSpace` object on success; NULL on failure.

## See Also

### Miscellaneous

clearNodeFlags

Resets the node's characteristics.

createPhysicalAddressSpace

Creates local physical FireWire address spaces for the device to access.

getNodeFlags

Retrieves the node's characteristics.

getUnitCount

Returns number of units attached to this device.

init

Initializes the nub.

setMaxSpeed

Sets the maximum speed for this node.

setNodeFlags

Sets the node's characteristics.

