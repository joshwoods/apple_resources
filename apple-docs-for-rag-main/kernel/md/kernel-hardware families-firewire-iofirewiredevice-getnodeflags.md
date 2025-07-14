

- Kernel
- Hardware Families
- FireWire
- IOFireWireDevice
-  getNodeFlags 

# getNodeFlags

Retrieves the node's characteristics.

``` source
virtual UInt32 getNodeFlags(
 flags ); 
```

## Parameters 

`flags`  

Refer to "node flags" in IOFireWireFamilyCommon.h.

## Return Value

UInt32 The flags set for a particular node.

## See Also

### Miscellaneous

clearNodeFlags

Resets the node's characteristics.

createPhysicalAddressSpace

Creates local physical FireWire address spaces for the device to access.

createPseudoAddressSpace

Creates local pseudo FireWire address spaces for the device to access.

getUnitCount

Returns number of units attached to this device.

init

Initializes the nub.

setMaxSpeed

Sets the maximum speed for this node.

setNodeFlags

Sets the node's characteristics.

